---
id: "section_N2539484"
type: "section"
title: "UpdateQuantity.ss"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Create and Use SSP Applications > SuiteScript 1.0 SSP Applications > Sample SSP Application Code (SuiteScript 1.0) > UpdateQuantity.ss"
parent: "section_N2538995"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539484.html"
anchors: []
sha256: "1d52a511c34d2bfd2311d5418820f9942ad911f20282f5d4fbe7e86195e91140"
---

Note:

For more information on SuiteScript 1.0, see [SuiteScript 1.0 Guide.](https://system.netsuite.com/app/help/helpcenter.nl?fid=SuiteScript10.pdf)

The following code contains the backend function for updating quantity in the Cart\_WithService .ssp file:

          `function service(request,response) {    // get incoming http parameter    var quantity = request.getParameter('quantity');    nlapiLogExecution('DEBUG', 'quantity', quantity);        // get active order in web container       var order = nlapiGetWebContainer().getShoppingSession().getOrder();           // get the items out of the order    var items = order.items;        var orderItemId = items[0].orderitemid;    nlapiLogExecution('DEBUG', 'order item id - line 1', orderItemId);        var currentQuantityLine1 = items[0].quantity;    nlapiLogExecution('DEBUG', 'order curr qty - line 1', currentQuantityLine1);      var updatedItem = new Object();    updatedItem.orderitemid = orderItemId;    updatedItem.quantity = quantity;        order.updateItemQuantity(updatedItem);      var itemsJSON = JSON.stringify(order.getItems());           // send items back out as JSON,     response.setContentType('JSON');    response.writeLine(itemsJSON);    }` 
        

### Related Topics

-   [Sample\_Cart.ssp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539246.html)
-   [Cart\_WithService.ssp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539373.html)
-   [AddCartItem.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539594.html)
-   [AddCustomerAddress.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539614.html)
-   [Example .ss File Code that Accesses a NetSuite Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539634.html)
-   [ItemOption.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3746220243.html)
-   [Known Issue with Internet Explorer and Plain Text Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539732.html)
-   [Sample SSP Application Code (SuiteScript 1.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2538995.html)
-   [SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529595280.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
