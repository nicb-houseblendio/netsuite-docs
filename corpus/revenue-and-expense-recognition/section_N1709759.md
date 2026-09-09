---
id: "section_N1709759"
type: "section"
title: "Creating a Revenue Commitment Reversal from a Return Authorization"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Commitments > Creating Revenue Commitment Reversals > Creating a Revenue Commitment Reversal from a Return Authorization"
parent: "section_N1709562"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1709759.html"
anchors: ["procedure_N1709790"]
sha256: "973dba5eca4a9e042fcad10cb69b469f9addb779e1ffe89bb2a5dce9f976728a"
---

Important:

The functions discussed in this topic require the Revenue Commitments feature to be enabled.

This process is similar to creating a revenue commitment from a sales order. For information about that process, see [Creating a Revenue Commitment from a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707177.html).

A return authorization provides the basic information used to create and populate a revenue commitment reversal. For information about return authorizations, see [Customer Returns Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1303799.html). You can't add items to a revenue commitment reversal that don't appear on the return authorization.

#### To create a revenue commitment reversal directly from a return authorization: {#procedure_N1709790}

1.  After providing all of the information required on a Return Authorization page, on the **Accounting** subtab, check the **Rev Rec on Commit** box. This tells NetSuite to use a revenue commitment reversal to reverse revenue for **all** lines on this return authorization.
    
    After NetSuite creates an invoice, cash sale, or revenue commitment, NetSuite also disables the **Rev Rec on Rev Commit.** box. At that point, the only way to disable the Revenue Recognition on Revenue Commitment option is to delete all of the child transactions.
    
2.  Click **Reverse Revenue** to open the New Revenue Commitment Reversal page.
    
3.  In Primary Information, if autonumbering is disabled, optionally enter an identification number in the **Rev. Commitment Reversal #** field and any other information not included on the return authorization that you want on the revenue commitment reversal.
    
4.  Complete fields on each of the following subtabs, as necessary.
    
    -   **Items**
        
    -   **Accounting**
        
    -   **Sales Team**
        
    -   **Address**
        
    -   **Custom**
        
    
    To avoid reporting differences between return authorizations and the revenue commitment reversals derived from them, you generally shouldn't change the values populated into the revenue commitment reversal from the return authorization.
    

### Related Topics

-   [Creating Revenue Commitment Reversals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1709562.html)
-   [Using the Generate Revenue Commitment Reversals Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1709968.html)
-   [Return Authorization (RMA) Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1304530.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
