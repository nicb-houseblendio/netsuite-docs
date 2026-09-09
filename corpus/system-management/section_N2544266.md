---
id: "section_N2544266"
type: "section"
title: "Integrating with 3D Secure (SCA Elbrus and Earlier)"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Integration with Third-Party Checkout Providers > Integrating with 3D Secure (SCA Elbrus and Earlier)"
parent: "section_N2539882"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2544266.html"
anchors: ["bridgehead_N2544408", "bridgehead_N2544422", "bridgehead_N2544435", "bridgehead_3951128155", "bridgehead_3951129589", "bridgehead_3951615841"]
sha256: "a52226470b3675f0cc9283e958ad706d13c16f8ef62df9e394a6a3f5b94b81b5"
---

Warning:

This topic is only for 3D Secure 1. Support for 3D Secure 1 ended on October 15, 2022. If you rely on 3D Secure 1 for your SuiteCommerce Advanced web store, you'll probably see more failed or declined payment card transactions. See [End of Support for 3D Secure 1](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_070511571310.html) for more information, including information about migrating your website technologies from 3D Secure 1 to 3D Secure 2.

Sites running the Elbrus release of SuiteCommerce Advanced or earlier don't support 3D Secure. To add 3D Secure 1.0 to these versions, you'll need to either upgrade to the latest SCA release or follow the customization steps for the **Proceed to Checkout** touch point.

In an .ss file, call the submit method on the order shopping object, and pass these `paymentauthorization` object fields as [checkoutsettings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2516589.html) parameters:

-   `type` - set to 'threedsecure'.
    
-   `noredirect` - Tells the platform to return a status object with the required 3D Secure fields instead of redirecting when 3D Secure authorization is needed (default is F).
    
    Note the following:
    
    -   If `noredirect` is set to F [threedsecure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2536058.html) , the redirect goes to the default 3D Secure authorization page.
        
    -   If `noredirect` is set to T when 3D Secure authorization is needed, the submit method returns an error status with a reason code of ERR\_WS\_REQ\_PAYMENT\_AUTHORIZATION and values for the paymentauthorization JSON object. You can use these values to handle the 3D Secure integration .
        
-   `termurl` - The URL for your client-side handler to process the 3D Secure callback and submit the order with the 3D Secure response.
    

Besides the .ss file, 3D Secure 1 integration needs client-side code to show 3D Secure information in the UI and handle orders. For code examples, see the following:

-   [Sample .ss File for 3D Secure 1 Integration](#bridgehead_N2544408)
    
-   [Sample for Adding 3D Secure 1 iFrame in User Interface](#bridgehead_N2544422)
    
-   [Sample Client-Side Handler for 3D Secure 1 Order Submission](#bridgehead_N2544435)
    
-   [sampleShoppingLib.js](#bridgehead_3951128155)
    
-   [sampleClientLib.js](#bridgehead_3951129589)
    
-   [samplePaypalCheckout.ss](#bridgehead_3951615841)
    

Note:

Integration with third-party checkout providers is not available for SSP applications written in SuiteScript 2.0. For more information about SuiteScript 1.0, see [SuiteScript 1.0 Guide.](https://system.netsuite.com/app/help/helpcenter.nl?fid=SuiteScript10.pdf)

## Sample .ss File for 3D Secure 1 Integration {#bridgehead_N2544408}

          `function service(request,response) {    var returnval = null;        try    {       var shoppingSession = nlapiGetWebContainer().getShoppingSession();              var shipMethod = shoppingSession.getOrder().getShippingMethod();              if (!shipMethod || !shipMethod.shipMethod)       {          var shipMethods = shoppingSession.getOrder().getAvailableShippingMethods();          nlapiLogExecution("DEBUG", "setShippingMethod", JSON.stringify(shipMethods));          shoppingSession.getOrder().setShippingMethod(shipMethods[0]);       }              var orderHandlerUrl = shoppingSession.getAbsoluteUrl('checkout', 'samplePlaceOrder.ss');       var orderSetting = {paymentauthorization:{type: 'threedsecure', noredirect : 'T', termurl : orderHandlerUrl}};       returnval = shoppingSession.getOrder().submit(orderSetting);    }    catch (e)    {       var nle = nlapiCreateError(e);       returnval = {status : 'error', reasoncode : nle.getCode(), message : nle.getDetails()};    }    response.writeLine(JSON.stringify(returnval));` 
        

## Sample for Adding 3D Secure 1 iFrame in User Interface {#bridgehead_N2544422}

          `<html> <head><%=getPageFullHead()%> <!--add css, js packages here --> <link rel="stylesheet" type="text/css" href="https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/css/style2.css" > <script language='JavaScript' type='text/javascript'> try {    if (window.parent != window && window.parent.document.getElementById('threedsecureframe') != null) { window.parent.location.href = window.location.href; }    } catch(e){ } </script> <script type="text/javascript" src="https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/lib/sampleShoppingLib.js"></script> <script type="text/javascript" src="https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/lib/sampleClientLib.js"></script> </head>    <body onLoad="loadShoppingCart();">  <table cellpadding=0 cellspacing=0 border=0 width=100%><NLPAGETOP></table>  <%nlapiGetWebContainer().getPageGenerator().setSelectedTab(3);%> <table width="100%"> <tr> <td><div></div></td> </tr> </table> <table border=0> <% var checkoutSettings = nlapiGetWebContainer().getShoppingSession().getSiteSettings(['checkout']);  var paypalUrl = nlapiGetWebContainer().getShoppingSession().getAbsoluteUrl("checkout", "samplePaypalCheckout.ss"); <tr> <td> <input type="submit" name="placeorder" value="Submit" onclick="placeOrder()"> </td> <td>&nbsp;</td> <td > <form name='paypalform' action='<%=paypalUrl%>' method='post'> <input type='image' src='<%=checkoutSettings.checkout.paypalexpress.imageurl%>'/> </form> </a> </td> </tr> </table> <div></div> </body> </html>` 
        

## Sample Client-Side Handler for 3D Secure 1 Order Submission {#bridgehead_N2544435}

          `function placeOrderCallBack(req) {     var responseObj = JSON.parse(req.responseText);     if (responseObj.statuscode && responseObj.statuscode == "error")     {         // Order is not successful since payment authorization is required         if (responseObj.reasoncode && responseObj.reasoncode == "ERR_WS_REQ_PAYMENT_AUTHORIZATION")         {             if (responseObj.paymentauthorization)             {                 // grab the frame html for threedsecure and inject it into the page. this will trigger the autherization flow                 document.getElementById('paymentauthenticator').innerHTML = responseObj.paymentauthorization.servicehtml;                 var placeOrderBtn = document.getElementById('placeorder');                 if (placeOrderBtn)                     placeOrderBtn.parentNode.removeChild(placeOrderBtn);                 var paypalBtn = document.getElementById('paypalcheckout');                 if (paypalBtn)                     paypalBtn.parentNode.removeChild(paypalBtn);                              }         }     }   }` 
        

          `function service(request,response) {    var returnval = null;      try    {       var shoppingSession = nlapiGetWebContainer().getShoppingSession();       var orderHandlerUrl = shoppingSession.getAbsoluteUrl('checkout', 'samplePlaceOrder.ss');         var orderSetting = {paymentauthorization:{type: 'threedsecure', noredirect : 'T', termurl : orderHandlerUrl}};         returnval = shoppingSession.getOrder().submit(orderSetting);   }    catch (e)    {       var nle = nlapiCreateError(e);       returnval = {status : 'error', reasoncode : nle.getCode(), message : nle.getDetails()};    }    response.writeLine(JSON.stringify(returnval));` 
        

          `function placeOrderCallBack(req) {    var responseObj = JSON.parse(req.responseText);    if (responseObj.statuscode && responseObj.statuscode == "error")    {       // Order is not success since payment autherization is required       if (responseObj.reasoncode && responseObj.reasoncode == "ERR_WS_REQ_PAYMENT_AUTHORIZATION")       {          if (responseObj.paymentauthorization)          {             // grab the frame html for threedsecure and inject it into the page. this will trigger the autherization flow             document.getElementById('paymentauthenticator').innerHTML = responseObj.paymentauthorization.servicehtml;             var placeOrderBtn = document.getElementById('placeorder');             if (placeOrderBtn)                placeOrderBtn.parentNode.removeChild(placeOrderBtn);             var paypalBtn = document.getElementById('paypalcheckout');             if (paypalBtn)                paypalBtn.parentNode.removeChild(paypalBtn);          }       }    }   }` 
        

## sampleShoppingLib.js {#bridgehead_3951128155}

          `function createCartItemRow(nlCartItem, itemAttributes) {    var row = document.createElement('tr');        for (var i = 0; i < itemAttributes.length; i++)    {       row.appendChild(createCartItemCell(getCartItemAttributeText(itemAttributes[i], nlCartItem[itemAttributes[i]])));    }     return row; } function getCartItemAttributeText(attrName, attrValue) {    if (attrName === 'options')    {       var attrText = '';       if (attrValue)       {          for (var i = 0; i < attrValue.length; i++)          {             var itemOption = attrValue[i];             attrText += itemOption.name + ':' + itemOption.displayvalue + '\n';          }       }       return attrText;    }    else       return attrValue; }  function createCartItemCell(nlCartItemAttr) {    var cell = document.createElement('td');    cell.setAttribute('class', 'texttable');    var txtCell = document.createTextNode(nlCartItemAttr);    cell.appendChild(txtCell);    return cell; }  function createCartTableHeader(headerItems) {    var theader = document.createElement('thead');    theader.setAttribute('id', 'carttableheader');    for (var i = 0; i < headerItems.length; i++)    {       theader.appendChild(createCartHeaderCell(headerItems[i]));    }    return theader; } function createCartHeaderCell(nlCartHeaderItem) {    var cell = document.createElement('th');    var txtCell = document.createTextNode(nlCartHeaderItem);    cell.appendChild(txtCell);    return cell; }  function createShoppingCart(nlShoppingOrder) {       var headerItems = ['Name', 'Description', 'Options', 'Quantity', 'Rate', 'Amount'];    var itemAttributes = ['name', 'salesdesc', 'options', 'quantity', 'rate', 'amount'];       var shoppingCart = document.createElement('table');    shoppingCart.setAttribute('id', 'carttable');    shoppingCart.setAttribute('width', '100%');        var theader = createCartTableHeader(headerItems);    shoppingCart.appendChild(theader);     var tbody = document.createElement('tbody');        if (nlShoppingOrder && nlShoppingOrder.items)    {       for (var i = 0; i < nlShoppingOrder.items.length; i++)       {          tbody.appendChild(createCartItemRow(nlShoppingOrder.items[i], itemAttributes));       }    }     shoppingCart.appendChild(tbody);    document.getElementById('mainContents').appendChild(shoppingCart); }  function loadShoppingCart() {    sendRequest('sampleGetOrderFields.ss', loadShoppingCartCallback);    sendRequest('sampleGetCheckoutUrl.ss', loadCheckoutSettingCallback); }  function loadCheckoutSetting() {    sendRequest('sampleGetCheckoutUrl.ss', loadCheckoutSettingCallback); }  function loadCheckoutSettingCallback(req) {    var checkoutSetting = JSON.parse(req.responseText);    var paypalBtn = document.getElementById('paypalcheckout');    if (paypalBtn)       paypalBtn.href = checkoutSetting.paypalexpress;    }  function loadShoppingCartCallback(req) {    //render the items table    var order = JSON.parse(req.responseText);    createShoppingCart(order); }  function placeOrder()  {    sendRequest('samplePlaceOrder.ss', placeOrderCallBack); } function placeOrderCallBack(req) {       var responseObj = JSON.parse(req.responseText);    if (responseObj.statuscode && responseObj.statuscode == "error")    {       // Order is not success since payment autherization is required       if (responseObj.reasoncode && responseObj.reasoncode == "ERR_WS_REQ_PAYMENT_AUTHORIZATION")       {          if (responseObj.paymentauthorization)           {             // grab the frame html for threedsecure and inject it into the page. this will trigger the autherization flow             document.getElementById('paymentauthenticator').innerHTML = responseObj.paymentauthorization.servicehtml;             var placeOrderBtn = document.getElementById('placeorder');             if (placeOrderBtn)                placeOrderBtn.parentNode.removeChild(placeOrderBtn);             var paypalBtn = document.getElementById('paypalcheckout');             if (paypalBtn)                paypalBtn.parentNode.removeChild(paypalBtn);          }       }    }  }` 
        

## sampleClientLib.js {#bridgehead_3951129589}

          `function sendRequest(url,callback,postObjName, postData) {    var req = createXMLHTTPObject();    if (!req) return;    var method = (postData) ? "POST" : "GET";    req.open(method,url,true);    req.setRequestHeader('User-Agent','XMLHTTP/1.0');    if (postData) {       req.setRequestHeader('Content-type','application/x-www-form-urlencoded');       req.setRequestHeader(postObjName, JSON.stringify(postData));       }    req.onreadystatechange = function () {       if (req.readyState != 4) return;       if (req.status != 200 && req.status != 304) { //         alert('HTTP error ' + req.status);          return;       }       callback(req);    }    if (req.readyState == 4) return;    req.send();    //req.send(postData); }  var XMLHttpFactories = [    function () {return new XMLHttpRequest()},    function () {return new ActiveXObject("Msxml2.XMLHTTP")},    function () {return new ActiveXObject("Msxml3.XMLHTTP")},    function () {return new ActiveXObject("Microsoft.XMLHTTP")} ];  function createXMLHTTPObject() {    var xmlhttp = false;    for (var i=0;i<XMLHttpFactories.length;i++) {       try {          xmlhttp = XMLHttpFactories[i]();       }       catch (e) {          continue;       }       break;    }    return xmlhttp; }` 
        

## samplePaypalCheckout.ss {#bridgehead_3951615841}

          `function service(request,response) {    var returnval = null;        try    {              var shoppingSession = nlapiGetWebContainer().getShoppingSession();       var siteSetting = shoppingSession.getSiteSettings(['touchpoints']);           var viewcart = siteSetting.touchpoints.viewcart;       var homeurl = siteSetting.touchpoints.home;       var checkouturl = siteSetting.touchpoints.checkout;              var testUrl = shoppingSession.getAbsoluteUrl('/sampleGcoCheckout.ss');       var testUrl2 = shoppingSession.getAbsoluteUrl('lib/sampleShoppoingLib.js');           var paypalSetting = {type: 'paypalexpress', continueurl : checkouturl, cancelurl : viewcart};           nlapiGetWebContainer().getShoppingSession().proceedToCheckout(paypalSetting);    }    catch (e)    {       var nle = nlapiCreateError(e);       returnval = {status : 'error', reasoncode : nle.getCode(), message : nle.getDetails()};              response.writeLine(JSON.stringify(returnval));    } }` 
        

### Related Topics

-   [Integrating with PayPal Express](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2540093.html)
-   [Integration with Third-Party Checkout Providers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539882.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
