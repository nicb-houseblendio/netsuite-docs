---
id: "section_N2539614"
type: "section"
title: "AddCustomerAddress.ss"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Create and Use SSP Applications > SuiteScript 1.0 SSP Applications > Sample SSP Application Code (SuiteScript 1.0) > AddCustomerAddress.ss"
parent: "section_N2538995"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539614.html"
anchors: []
sha256: "b3984ca10d5ced61c52ff763c71b81d2f4809bab58bbd1d97c34c0ee8ae539c4"
---

Note:

For more information on SuiteScript 1.0, see [SuiteScript 1.0 Guide.](https://system.netsuite.com/app/help/helpcenter.nl?fid=SuiteScript10.pdf)

          `function service(request,response) {   /*var addressee = request.getParameter('addressee');   var addr1 = request.getParameter('addr1');   var city = request.getParameter('city');   var state = request.getParameter('state');   var zip = request.getParameter('zip');   var country = request.getParameter('country');   var phone = request.getParameter('phone');     var address = {     addressee : addressee,     addr1 : addr1,     city : city,     state : state,     zip : zip,     country : country,     phone : phone,     defaultshipping : 'T',     defaultbilling : 'T'   };*/     // Or the object string can be passed from the request header   var address = JSON.parse(request.getHeader('customerAddress'));     // Get a reference to the customer   var customer = nlapiGetWebContainer().getShoppingSession().getCustomer();     try   {     // Add the address     var status = customer.addAddress(address);       var result = customer.getFieldValues();       // return the customer data through response     response.writeLine(JSON.stringify(result.customer));   }   catch (e)   {     var e2 = nlapiCreateError(e);     // Do error handling here   } }` 
        

### Related Topics

-   [Sample\_Cart.ssp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539246.html)
-   [Cart\_WithService.ssp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539373.html)
-   [UpdateQuantity.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539484.html)
-   [AddCartItem.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539594.html)
-   [Example .ss File Code that Accesses a NetSuite Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539634.html)
-   [ItemOption.ss](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3746220243.html)
-   [Known Issue with Internet Explorer and Plain Text Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539732.html)
-   [Sample SSP Application Code (SuiteScript 1.0)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2538995.html)
-   [SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529595280.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
