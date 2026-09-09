---
id: "section_N2539373"
type: "section"
title: "Cart_WithService.ssp"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Create and Use SSP Applications > SuiteScript 1.0 SSP Applications > Sample SSP Application Code (SuiteScript 1.0) > Cart_WithService.ssp"
parent: "section_N2538995"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539373.html"
anchors: []
sha256: "c2b4e888f683bad7492ae44d6d4c03af560325b2303dd4c508332fdeb12ec7a2"
---

Note:

For more information on SuiteScript 1.0, see [SuiteScript 1.0 Guide.](https://system.netsuite.com/app/help/helpcenter.nl?fid=SuiteScript10.pdf)

The following code creates a View Cart touchpoint that references an UpdateQuantity backend function. To work, this code requires the UpdateQuantity.ss file.

          `<html> <head>    <%=getPageFullHead()%> <script language="JavaScript">   var xmlhttp = new XMLHttpRequest();      /*  * Dynamically build out the cart header  */    function buildCartHeader() {      var tHead = cartTable.createTHead();      var row, cell;        row = tHead.insertRow(-1);      tHead.setAttribute("bgColor","lightskyblue");       cell = row.insertCell(-1);     cell.align = "center";     cell.style.fontWeight = "bold";     cell.innerHTML = 'Item';         cell = row.insertCell(-1);     cell.align = "center";     cell.style.fontWeight = "bold";     cell.innerHTML = 'QTY';       cell = row.insertCell(-1);     cell.align = "center";     cell.style.fontWeight = "bold";     cell.innerHTML = 'Rate';       cell = row.insertCell(-1);     cell.align = "center";     cell.style.fontWeight = "bold";     cell.innerHTML = 'Amount';    }   /*  * Dynamically build out the cart  */ function buildCartItems(items) {   var row, cell;            // Insert table rows and cells into body   for (var i=0; i<items.length; i++)   {     row = cartBody.insertRow(-1);      cell = row.insertCell(-1);        cell.innerHTML = items[i].name;        cell = row.insertCell(-1);      cell.innerHTML = items[i].quantity;        cell = row.insertCell(-1);      cell.innerHTML = items[i].rate;        cell = row.insertCell(-1);      cell.innerHTML = items[i].amount;   }     // Set the background color of the table body.   cartBody.setAttribute("bgColor","white"); }   /*  * Process result of AJAX call to update quantity  */ function handleServiceResponse() {    if (xmlhttp.readyState == 4 && xmlhttp.status == 200)     {       // remove the cart contents       document.getElementById('cartBody').innerHTML = '';              // parse the JSON result into JavaScript objects,       // and rebuild the cart       var items = JSON.parse(xmlhttp.responseText);       buildCartItems(items);             }    }   /*  * AJAX call to NetSuite service  * Service updates the quantity on line 1  */ function updateQuantity() {         xmlhttp.onreadystatechange=handleServiceResponse;         xmlhttp.open('POST', 'updateQuantity.ss', true);           xmlhttp.setRequestHeader('Content-type','application/x-www-form-urlencoded');      try    {       xmlhttp.send('quantity=' +    document.getElementById('quantity').value);      }     catch (ex)      {       alert(ex);      }    }   </script> </head> <body>     <table cellpadding=0 cellspacing=0 border=0 width=100%>    <%=getPageTop()%> </table>   <button type="button" onclick="updateQuantity();">Update    QTY(line1)</button> <input type="text"/>   <br><br>     <table border="1" bgcolor="lightslategray">    <tbody></tbody> </table>   <script language="JavaScript"> <%var order = nlapiGetWebContainer().getShoppingSession().getOrder();%>   // JSON.parse not used here since client script is generated similar to... //     var items = '[{"itemid":"Urban Dining Table","onlinecustomerprice":"1686.26"' // Setting a variable explicitly equal to a JSON string automatically converts to    objects var items = <%=JSON.stringify(order.getItems())%>   buildCartHeader(); buildCartItems(items);   </script>   </body> </html>` 
        

### Related Topics

-   [Sample\_Cart.ssp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539246.html)
-   [UpdateQuantity.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539484.html)
-   [AddCartItem.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539594.html)
-   [AddCustomerAddress.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539614.html)
-   [Example .ss File Code that Accesses a NetSuite Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539634.html)
-   [ItemOption.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3746220243.html)
-   [Known Issue with Internet Explorer and Plain Text Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539732.html)
-   [Sample SSP Application Code (SuiteScript 1.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2538995.html)
-   [SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529595280.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
