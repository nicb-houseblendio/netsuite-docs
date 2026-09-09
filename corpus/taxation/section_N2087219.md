---
id: "section_N2087219"
type: "section"
title: "Recording Withholding Taxes on Transactions as a Seller"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Withholding Tax > Recording Withholding Taxes on Transactions as a Seller"
parent: "chapter_N2078886"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087219.html"
anchors: []
sha256: "ef42d956ba7eb7d0c11211af6bc2d7cc69786061a1be7eeffa6c99ec46b29524"
---

Important:

The topics here cover withholding tax for NetSuite accounts without the SuiteTax feature enabled. If you're using an account with SuiteTax enabled, go to [Withholding Taxes in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159646451288.html).

Withholding tax isn't getting new features and reports in accounts without SuiteTax. Updates to the Withholding Tax SuiteApp now include only fixes for reported issues.

You can record withholding taxes as a seller on invoice creation, on acceptance of payments, or on cash sales.

-   If your withholding tax setup has Tax Point = On Accrual, then withholding tax is recognized upon saving the invoice. See [Withholding Taxes on Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087402.html).
    
    Note:
    
    The Withholding Tax SuiteApp doesn't support bulk processing of invoices. You must edit and save each invoice to trigger the calculation of withholding tax.
    
-   If your withholding tax setup has Tax Point = On Payment, then withholding tax is recognized when the customer pays the invoice, and on cash sale transactions. See [Withholding Taxes on Payment Acceptance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087711.html) and [Withholding Taxes on Cash Sales](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2088149.html).
    

Important:

If Tax Point = On Payment, and if Available on Sales is checked in your Withholding Tax Setup, NetSuite makes sure the withholding tax calculation matches the amount posted in the general ledger by locking the withholding tax credit memos and their associated invoices when payment has been applied. You can still unapply, cancel or delete a payment to make the related withholding tax credit memo and the associated invoice editable again. Note that when you delete an invoice payment, the associated credit memo to record withholding tax in the GL is also deleted. If Available on Sales is not checked, the withholding tax credit memos and the associated invoices become editable, regardless if withholding tax has been associated with the transaction.

### Related Topics

-   [Withholding Taxes on Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087402.html)
-   [Withholding Taxes on Payment Acceptance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087711.html)
-   [Withholding Taxes on Cash Sales](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2088149.html)
-   [Withholding Tax Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079416.html)
-   [Setting Up Withholding Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079716.html)
-   [Creating or Customizing Roles to Use Withholding Tax Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2080358.html)
-   [Setting Default Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085546.html)
-   [Applying Withholding Taxes on Transactions as a Buyer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085924.html)
-   [Importing Withholding Tax Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4606135691.html)
-   [Withholding Tax Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2088848.html)
-   [Withholding Tax Troubleshooting Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4485199528.html)
-   [Known Limitations of the Withholding Tax SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160458601048.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
