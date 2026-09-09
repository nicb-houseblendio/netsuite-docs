---
id: "section_N2085924"
type: "section"
title: "Applying Withholding Taxes on Transactions as a Buyer"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Withholding Tax > Applying Withholding Taxes on Transactions as a Buyer"
parent: "chapter_N2078886"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085924.html"
anchors: []
sha256: "a18a4bb05c418af7d4b5ba92ca0b32ce7985658bbff3b56e068158e96cca8342"
---

Important:

The topics here cover withholding tax for NetSuite accounts without the SuiteTax feature enabled. If you're using an account with SuiteTax enabled, go to [Withholding Taxes in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159646451288.html).

Withholding tax isn't getting new features and reports in accounts without SuiteTax. Updates to the Withholding Tax SuiteApp now include only fixes for reported issues.

You can record withholding taxes as a buyer when you create of vendor bills or checks.

-   If your withholding tax setup has Tax Point = On Accrual, when you save the bill, withholding tax amounts are posted automatically to the proper appropriate general ledger accounts. See [Withholding Taxes on Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2086130.html).
    
-   If your withholding tax setup uses Tax Point = On Payment, withholding tax is recognized when you pay the bill. For more information, see [Withholding Taxes on Bill Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2086435.html) and [Withholding Taxes on Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2086925.html).
    

Important:

If Tax Point = On Payment, and Available on Purchases is checked in your Withholding Tax Setup, NetSuite makes sure the withholding tax calculation matches the amount posted in the general ledger by locking the withholding tax vendor credits and their associated bills when payment has been applied. You can still unapply, cancel or delete a bill payment to make the related withholding tax vendor credit and associated bill editable. Note that when you delete a bill payment, the associated vendor credit to record withholding tax in the GL is also deleted. If Available on Purchases is not checked, the withholding tax vendor credits and the associated bills become editable, regardless if withholding tax has been associated with the transaction.

### Related Topics

-   [Withholding Taxes on Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2086130.html)
-   [Withholding Taxes on Bill Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2086435.html)
-   [Withholding Taxes on Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2086925.html)
-   [Withholding Tax Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079416.html)
-   [Setting Up Withholding Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079716.html)
-   [Creating or Customizing Roles to Use Withholding Tax Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2080358.html)
-   [Setting Default Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085546.html)
-   [Recording Withholding Taxes on Transactions as a Seller](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087219.html)
-   [Importing Withholding Tax Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4606135691.html)
-   [Withholding Tax Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2088848.html)
-   [Withholding Tax Troubleshooting Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4485199528.html)
-   [Known Limitations of the Withholding Tax SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160458601048.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
