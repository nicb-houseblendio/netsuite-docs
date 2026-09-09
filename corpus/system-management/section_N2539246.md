---
id: "section_N2539246"
type: "section"
title: "Sample_Cart.ssp"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Create and Use SSP Applications > SuiteScript 1.0 SSP Applications > Sample SSP Application Code (SuiteScript 1.0) > Sample_Cart.ssp"
parent: "section_N2538995"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539246.html"
anchors: []
sha256: "12a66c27cdfbeda50e970671632bd5216da4909158580809e460f4f0b42b996f"
---

Note:

For more information on SuiteScript 1.0, see [SuiteScript 1.0 Guide.](https://system.netsuite.com/app/help/helpcenter.nl?fid=SuiteScript10.pdf)

The following code creates a very basic View Cart touchpoint:

          `<html> <head><%=getPageFullHead()%> <!--add css, js packages here --> <link rel="stylesheet" type="text/css" href="https://docs.oracle.com/checkout/css/style2.css" > <% var order = nlapiGetWebContainer().getShoppingSession().getOrder().getFieldValues({'items': ['name', 'salesdesc', 'quantity', 'rate', 'amount'], 'summary': ''});%> <script type="text/javascript"> var nlShoppingOrder = <%=JSON.stringify(order)%>; </script>    <script type="text/javascript">    function createCartItemRow(nlCartItem, itemAttributes)    {       var row = document.createElement('tr');              for (var i = 0; i < itemAttributes.length; i++)       {          row.appendChild(createCartItemCell(nlCartItem[itemAttributes[i]]));       }         return row;    }    function createCartItemCell(nlCartItemAttr)    {       var cell = document.createElement('td');       cell.setAttribute('class', 'texttable');       var txtCell = document.createTextNode(nlCartItemAttr);       cell.appendChild(txtCell);       return cell;    }        function createCartTableHeader(headerItems)    {       var theader = document.createElement('thead');       theader.setAttribute('id', 'carttableheader');       for (var i = 0; i < headerItems.length; i++)       {          theader.appendChild(createCartHeaderCell(headerItems[i]));       }       return theader;    }    function createCartHeaderCell(nlCartHeaderItem)    {       var cell = document.createElement('th');       var txtCell = document.createTextNode(nlCartHeaderItem);       cell.appendChild(txtCell);       return cell;    }        function createShoppingCart()    {          var headerItems = ['Name', 'Description', 'Quantity', 'Rate', 'Amount'];       var itemAttributes = ['name', 'salesdesc', 'quantity', 'rate', 'amount'];          var shoppingCart = document.createElement('table');       shoppingCart.setAttribute('id', 'carttable');       shoppingCart.setAttribute('width', '100%');              var theader = createCartTableHeader(headerItems);       shoppingCart.appendChild(theader);         var tbody = document.createElement('tbody');              if (nlShoppingOrder && nlShoppingOrder.items)       {          for (var i = 0; i < nlShoppingOrder.items.length; i++)          {             tbody.appendChild(createCartItemRow(nlShoppingOrder.items[i], itemAttributes));          }       }         shoppingCart.appendChild(tbody);       document.getElementById('mainContents').appendChild(shoppingCart); }     </script> </head>    <body onLoad="createShoppingCart()">   <table cellpadding=0 cellspacing=0 border=0 width=100%><NLPAGETOP></table>   <table> <%nlapiGetWebContainer().getPageGenerator().setSelectedTab(3);%>   <div></div>   </table> </body> </html>` 
        

### Related Topics

-   [Cart\_WithService.ssp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539373.html)
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
