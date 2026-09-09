---
id: "section_N2539732"
type: "section"
title: "Known Issue with Internet Explorer and Plain Text Content"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Create and Use SSP Applications > SuiteScript 1.0 SSP Applications > Sample SSP Application Code (SuiteScript 1.0) > Known Issue with Internet Explorer and Plain Text Content"
parent: "section_N2538995"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539732.html"
anchors: []
sha256: "5b2e0e671760b77cad2fbd9f54f010ae67cf0f9d6111324cb2a7fc14f4080d8a"
---

If the content type for a file is set to text/plain in the HTTP header and the file name ends with .ssp or .ss extension (in the response header or URL), Internet Explorer might try to save the file instead of showing it inline.

This is a known issue with Internet Explorer 9 and might happen in earlier versions too. This issue doesn't happen with files that have HTML content instead of plain text.

Note:

For more information on SuiteScript 1.0, see [SuiteScript 1.0 Guide.](https://system.netsuite.com/app/help/helpcenter.nl?fid=SuiteScript10.pdf)

To ensure that Internet Explorer shows the file contents inline, use response.setContentType() to rename the file with a .txt extension, like in this example:

          `function service(request, response) {         response.setContentType('PLAINTEXT', 'my_SSP.txt', 'inline');         response.writeLine('hey'); }` 
        

### Related Topics

-   [Sample\_Cart.ssp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539246.html)
-   [Cart\_WithService.ssp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539373.html)
-   [UpdateQuantity.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539484.html)
-   [AddCartItem.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539594.html)
-   [AddCustomerAddress.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539614.html)
-   [Example .ss File Code that Accesses a NetSuite Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539634.html)
-   [ItemOption.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3746220243.html)
-   [Sample SSP Application Code (SuiteScript 1.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2538995.html)
-   [SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529595280.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
