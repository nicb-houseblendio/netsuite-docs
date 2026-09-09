---
id: "section_N2539882"
type: "section"
title: "Integration with Third-Party Checkout Providers"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Integration with Third-Party Checkout Providers"
parent: "preface_1521816133"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539882.html"
anchors: []
sha256: "abe54406ee8ae3f19e6180927443e19db767cb3e3ac4438b9b55164085faa032"
---

Note:

Integration with third-party checkout providers is not available for SSP applications written in SuiteScript 2.0. For more information about SuiteScript 1.0, see [SuiteScript 1.0 Guide.](https://system.netsuite.com/app/help/helpcenter.nl?fid=SuiteScript10.pdf)

To integrate with third-party checkout providers such as PayPal Express and 3D Secure, you'll need to create request handlers (.ss files) for them and call these handlers from your frontend page (.ssp file). The request handlers must use `proceedToCheckout()`, as documented in [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html). This method needs to pass [checkoutsettings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2516589.html) JSON object values as parameters. Note that you can only call from a secure (https) scheme. For more details, see:

-   [Integrating with PayPal Express](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2540093.html)
    
-   [Integrating with 3D Secure (SCA Elbrus and Earlier)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2544266.html)
    

Warning:

The help topic, [Integrating with 3D Secure (SCA Elbrus and Earlier)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2544266.html), applies to 3D Secure 1 only. Support for 3D Secure 1 ended on October 15, 2022. Relying on 3D Secure 1 for your Site Builder or SuiteCommerce Advanced web store is expected to result in more failed or declined payment card transactions. See [End of Support for 3D Secure 1](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_070511571310.html) for more information, including information about migrating your website technologies from 3D Secure 1 to 3D Secure 2.

### Related Topics

-   [SSP Application Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2490486.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)
-   [Debug a SuiteScript 1.0 SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495065.html)
-   [Bundle an SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495338.html)
-   [SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_1521816133.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
