---
id: "section_N2539634"
type: "section"
title: "Example .ss File Code that Accesses a NetSuite Record"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Create and Use SSP Applications > SuiteScript 1.0 SSP Applications > Sample SSP Application Code (SuiteScript 1.0) > Example .ss File Code that Accesses a NetSuite Record"
parent: "section_N2538995"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539634.html"
anchors: []
sha256: "84ec240d032a93e970e35227492e9041e95e3abe8f5001a723b297ff9adc883e"
---

Note:

For more information on SuiteScript 1.0, see [SuiteScript 1.0 Guide.](https://system.netsuite.com/app/help/helpcenter.nl?fid=SuiteScript10.pdf)

Code like the following can be used in an .ss file to access a NetSuite record rather than a shopping session object.

          `function service(request,response) {         var salesOrder = nlapiCreateRecord('salesorder', true);                  salesOrder.setFieldValue('customform', 88); // Cash Sale form.         salesOrder.setFieldValue('orderstatus', 'B');         salesOrder.selectNewLineItem('item');         salesOrder.setCurrentLineItemValue('item', 'item', 6);         salesOrder.setCurrentLineItemValue('item', 'quantity', 1);         salesOrder.setCurrentLineItemValue('item', 'rate', 500);         salesOrder.commitLineItem('item');         nlapiSubmitRecord(salesOrder); }` 
        

Important:

Running an .ss file with code accessing a NetSuite record requires a preexisting NetSuite session. Running this code without first logging in to NetSuite results in permission errors. Running this type of code from the shopping domain also results permission errors, because shoppers are only recognized in the shopping domain.

### Related Topics

-   [Sample\_Cart.ssp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539246.html)
-   [Cart\_WithService.ssp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539373.html)
-   [UpdateQuantity.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539484.html)
-   [AddCartItem.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539594.html)
-   [AddCustomerAddress.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539614.html)
-   [ItemOption.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3746220243.html)
-   [Known Issue with Internet Explorer and Plain Text Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539732.html)
-   [Sample SSP Application Code (SuiteScript 1.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2538995.html)
-   [SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529595280.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
