---
id: "section_N1702343"
type: "section"
title: "Setting Revenue Commitment Preferences"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Commitments > Setting Up the Revenue Commitments Feature > Setting Revenue Commitment Preferences"
parent: "section_N1702000"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1702343.html"
anchors: ["procedure_N1703184"]
sha256: "ecfd7a267fe98807d80dbf09b5b11130c35e2b054a7f109e0cf48a3145c3ef9d"
---

Important:

The functions discussed in this topic require the Revenue Commitments feature to be enabled.

The following accounting preferences are available when you enable the Revenue Commitments feature. These preferences are in addition to those available when the Revenue Recognition feature is enabled.

-   **Default Deferred Revenue Reclassification Account**
    
    Select the default deferred revenue account for reclassification between deferred revenue and unbilled receivable accounts at the order level. This account appears on customer records and on sales orders for that customer. You can override this default on the customer record or sales order.
    
    Note:
    
    With line level deferred revenue reclassification, the Deferred Revenue Reclassification account is used **only** to post order level deferred revenue until the order is fully billed and recognized. If you leave this field blank on a sales order, then order level deferred revenue is posted to the account set in this preference.
    
-   **Default Foreign Currency Adjustment Revenue Account**
    
    Select a default revenue account to post foreign currency adjustments that result when exchange rates are different for billing and revenue postings. You must select an income account. This account appears on customer records and on sales orders for the customer. You can override this default on the customer record or sales order.
    
    Note:
    
    The Foreign Currency Adjustment Revenue account isn't used when the line level deferred revenue reclassification enhancements for Version 2013 Release 2 are enabled for your account. The default account set here is ignored.
    
-   **Allow Revenue Commitments In Advance of Fulfillment**
    
    If this preference is enabled, then the Commit Revenue button appears on a transaction, such as a sales order, even if a transaction or the lines on it aren't fulfilled. Also, the Hide Unfulfilled Orders box appears in the Generate Revenue Commitments page.
    
    This preference is similar to the Invoicing preference called Invoice in Advance of Fulfillment, and as with that preference, NetSuite generates a Revenue Commitment for partially or completely fulfilled lines. For more information about the fulfillment process, see [Order Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1222915.html).
    
-   **Allow Revenue Commitment Reversals In Advance of Item Receipt**
    
    If this preference is enabled, then the Reverse Revenue button appears on a Return Authorization, even if the items to be returned haven't been received. Also, the Hide Unreceived Orders box appears in the Generate Revenue Commitments page. If this preference isn't checked, then the button doesn't appear. If this preference is disabled, then NetSuite only generates a Revenue Commitment Reversal. For more information about the return process, see [Customer Return Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1302852.html).
    

Depending on the other revenue features enabled, additional revenue recognition preferences may be available. Note that the following related preferences, when available, apply to revenue commitments:

-   Allow Users to Modify VSOE Values on Transactions
    
-   Prorate Revenue Recognition Dates for Partially Billed Sales Orders
    

The following preference doesn't apply to revenue commitments:

-   Adv. Billing Use Sales Order Amount.
    

For more information, see the [Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html#bridgehead_N1386651) section in [General Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html).

#### To set revenue commitments accounting preferences: {#procedure_N1703184}

1.  Go to _Setup > Accounting > Preferences > Accounting Preferences_.
    
2.  Click the **General** subtab, and scroll down to the Revenue Recognition and Classic Revenue Recognition Only sections of the page.
    
3.  Set preferences as desired, and click **Save**.
    

### Related Topics

-   [Setting Up the Revenue Commitments Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1702000.html)
-   [Enabling the Revenue Commitments Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1702170.html)
-   [Assigning Revenue Commitment Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1703344.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
