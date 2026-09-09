---
id: "section_N1707177"
type: "section"
title: "Creating a Revenue Commitment from a Sales Order"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Commitments > Creating Revenue Commitments > Creating a Revenue Commitment from a Sales Order"
parent: "section_N1707026"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707177.html"
anchors: ["procedure_N1707196"]
sha256: "96e75a50b1c63487a6448c1fbad276845ec908e44eddb921dce4342758218feb"
---

Important:

The functions discussed in this topic require the Revenue Commitments feature to be enabled.

Revenue commitments can only be created if a sales order exists. The sales order provides the basic information used to create and populate a revenue commitment. You can't add items to a revenue commitment that don't appear on the sales order.

#### To create a revenue commitment directly from a sales order: {#procedure_N1707196}

1.  After providing all of the information required on a sales order page, on the **Accounting** subtab, check the **Rev Rec on Rev Commit.** box. This preference tells NetSuite to use a revenue commitment to recognize revenue for **all** lines on this order and to use related invoices or cash sales solely for billing.
    
    For instructions for creating sales orders, see [Creating Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1216500.html).
    
    When NetSuite creates an invoice, cash sale, or revenue commitment, NetSuite also disables the Rev Rec on Rev Commit. box.
    
    ![Screenshot of the Accounting subtab of a sales order with the Rev Rec on Rev Commit. box checked and outlined in red](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/RevenueExpenseRecognition/AcctgTabSalesOrder.png)
2.  Click **Commit Revenue** to open the Revenue Commitment page. If your process includes order approval, the **Commit Revenue** button is available when the order is approved.
    
3.  In Primary Information, if autonumbering is disabled, optionally enter an identification number in the **Rev. Commitment #** field and any other information not included on the sales order that you want on the revenue commitment.
    
4.  Complete fields on each of the following subtabs as necessary. Because a revenue commitment functions like an invoice, these tabs and the fields on them are similar to those on a invoice. For more information, see [Understanding Revenue Commitment Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1708322.html).
    
    -   **Items**
        
    -   **Accounting**
        
    -   **Sales Team**
        
    -   **Address**
        
    -   **Custom**
        
    
    For more information about how to complete fields on these subtabs, see [Creating an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1238506.html).
    
    Important:
    
    To recognize revenue using a revenue commitment, all lines on a certain sales order must be included on one or more revenue commitments. You can't recognize revenue on sales orders using revenue commitments for some lines on the sales order and invoices to recognize revenue from other lines on the sales order. The same requirements apply to revenue commitment reversals and return authorizations.
    
5.  Click **Save**.
    

To avoid reporting differences between sales orders and the revenue commitments derived from them, you generally shouldn't change the values populated into the revenue commitment from the sales order. For example, if you set the Department on the sales order to R&D, and on the revenue commitment you set the Department to G & A, your reports may display different values for revenues and receivables.

A revenue commitment, like a sales order, is a non-posting transaction. It serves as the placeholder for the revenue recognition schedule that generates the posting revenue recognition journal entries.

### Related Topics

-   [Creating Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707026.html)
-   [Understanding Revenue Commitment Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1708322.html)
-   [Using the Generate Revenue Commitment Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707431.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
