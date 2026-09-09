---
id: "section_N1548500"
type: "section"
title: "Entering Company Credit Card Charges"
branch: "banking"
category: "accounting"
breadcrumb: "Accounting > Banking > Company Credit Cards > Entering Company Credit Card Charges"
parent: "chapter_N1548363"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1548500.html"
anchors: ["procedure_N1548521", "procedure_N1548617", "procedure_N1548676", "bridgehead_4382656902", "procedure_N1548731", "procedure_N1548754", "bridgehead_4382657423", "bridgehead_4382657670"]
sha256: "6d40e07cdb4499affd58b49111dbd5ad78a3777f55c398a7e66de1b29ee42be6"
---

To manage charges and payments for your company credit card, enter each transaction individually. Transactions post immediately.

To import credit card charges, see [Credit Card Charge Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4676571596.html).

To import bank or credit card statements, see [Bank Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1550803.html).

#### To enter credit card transactions: {#procedure_N1548521}

1.  If you want to record a purchase, go to _Transactions > Bank > Issue Credit Card Charge_.
    
    If you want to record a credit or a refund, go to _Transactions > Bank > Issue Credit Card Refund_
    
    Note:
    
    For credit type transactions like returned items, tax posts to GST or VAT on Purchases.
    
2.  Under Primary Information, enter a reference number from the credit card transaction if needed.
    
3.  In the **Vendor** field, select the entity you are paying or the entity crediting you for a previous purchase.
    
    The currency field defaults to the currency on the entity record.
    
    In NetSuite OneWorld, the subsidiary appears under Classification.
    
4.  In the **Account** field, select the credit card account for this transaction.
    
    The current balance of the credit card account appears in the **Balance** field.
    
    In NetSuite OneWorld, the list displays only credit card accounts with the same currency as the vendor.
    
    Note:
    
    The currency for a credit card account is always the currency of the subsidiary when the account was created. If you change the subsidiary to one with a different currency, the account keeps its original currency and is available only for transactions in that currency.
    
5.  In the **Amount** field, enter the amount of the transaction.
    
6.  Enter a different exchange rate if needed.
    
7.  The **Date** field displays the current date.
    
    Enter a different date if needed.
    
8.  If you use the **Accounting Period** feature, select a posting period.
    
    You can enter transactions only to open periods.
    
9.  Enter a memo if needed.
    

#### Expenses {#procedure_N1548617}

1.  Under **Expenses & Items**, on the **Expenses** subtab, select the expense account.
    
    Available expenses are filtered by the selected vendor and subsidiary.
    
    Important:
    
    The Unbilled Receivable account appears in the account list when the **Expand Account Lists** accounting preference is enabled. **Don't select this account**. All debits and credits must be system-generated.
    
2.  Enter the amount for the expense.
    
3.  Enter memo if needed.
    
4.  Enter a class, department, or location if needed.
    
5.  If the expense is billable to a customer, select the customer and check the **Billable** box.
    
6.  Click **Add**.
    
7.  Repeat these steps for each expense you want to add to this credit card charge.
    

#### Items {#procedure_N1548676}

1.  To add items, on the **Items** subtab, select an item name or click **Add Multiple** to quickly add several items.
    
    Available items are filtered by the selected vendor and subsidiary.
    
2.  Enter the item information.
    
    For details about entering item information, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).
    
    Note:
    
    If you use NetSuite OneWorld and share the selected vendor with multiple subsidiaries, the item price is based on the item definition for the vendor and subsidiary. Changing the subsidiary could change the item price.
    
3.  Click **Add**.
    
4.  Repeat these steps for each item you want to add to this credit card.
    

## Tax Details {#bridgehead_4382656902}

If VAT/GST nexuses and tax preferences are set in your NetSuite account, click the **Tax Details** subtab to select the vendor's nexus and tax registration number. Check the **Override** box to override vendor defaults, and then complete the tax lines.

## Relationships {#procedure_N1548731}

Click the **Relationships** subtab to add contact information. The primary contact is selected automatically. To edit this contact, click the contact's name. Add more contacts by entering their information and clicking **Add**.

## Communication {#procedure_N1548754}

-   Use the **Phone Calls**, **Events**, and **Tasks** subtabs to attach activities to the transaction. For more information, see [Attaching Events, Tasks, and Calls to Records and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1084924.html).
    
-   On the **Files** subtab, select and attach files related to the transaction. For more information, see [Attaching Files to Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N490137.html).
    
-   On the **User Notes** subtab, enter a title, memo date, time, type, and direction for any comments you want to add. Click **Add** after each note. For more information, see [Attaching Events, Tasks, and Calls to Records and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1084924.html).
    

The **Balance** field displays the current balance for the credit card account. After you enter each transaction, the account balance should match your credit card statement, unless you've made additional charges since the statement was printed.

## Accounting Books {#bridgehead_4382657423}

If you use NetSuite OneWorld and have **Multi-Book Accounting**, the Accounting Books subtab appears. This subtab shows secondary books for the selected vendor, if any, and their base currencies and exchange rates. For information about Multi-Book Accounting, see [Using Multi-Book Accounting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3831569045.html).

## Tax Reporting {#bridgehead_4382657670}

If you use the International Tax Reports SuiteApp, on the **Tax Reporting** subtab, select the delivery terms, region of origin, nature of transaction code, and mode of transport. Check the **Non-deductible Tax Adjusted** box if this check includes a nondeductible tax. For more information, see [EU Intrastat Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2069213.html).

**Save** the credit card transaction.

### Related Topics

-   [Creating Company Credit Card Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3758988949.html)
-   [Paying the Company Credit Card Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1548897.html)
-   [Reconciling Credit Card Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1550288.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
