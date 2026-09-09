---
id: "chapter_N3906699"
type: "chapter"
title: "FAQ: Accounting & ERP"
branch: "frequently-asked-questions"
category: "additional-resources"
breadcrumb: "Additional Resources > Frequently Asked Questions > FAQ: Accounting & ERP"
parent: "book_N3895042"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3906699.html"
anchors: ["question_N3906855", "question_N3908447", "question_N3908528", "procedure_N3908537", "question_N3908817", "procedure_N3908830", "procedure_N3908903", "question_N3909065"]
sha256: "aca71526532d62a48f3845e36dce1883c98f9111d69f49e898ba9a609737e8dd"
---

See the questions and answers below for information on Accounting & ERP.

### How do I record asset depreciation? {#question_N3906855}

**Fixed Asset Management**

NetSuite has a Fixed Assets Management bundle that provides automated management of fixed assets acquisition, depreciation, revaluation, and retirement, as well as maintenance schedules and insurance. You can import new assets and mid-life assets into NetSuite to track asset depreciation, including the depreciation history of mid-life assets. New asset records can also be created manually or from purchases, expenses, and inventory transfers in NetSuite. For more information, read the [Fixed Asset Management Guide](https://system.netsuite.com/app/help/helpcenter.nl?fid=FixedAssetsManagement.pdf). To purchase this add-on module, contact your NetSuite account manager.

### How do I close an accounting period? {#question_N3908447}

For detailed instructions on closing an accounting period, see [Accounting Period Close](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html).

### Related Topics:

-   [Accounting Period Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445585.html)

### How do I create a vendor prepayment? {#question_N3908528}

#### To create a vendor prepayment, complete the following three steps: {#procedure_N3908537}

1.  Create a holding account by following the instructions at [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html):
    
    1.  Go to _Setup > Accounting > Manage G/L > Chart of Accounts_.
        
    2.  Set the **Type** to **Expense**.
        
    3.  If you use account numbers assign this account a number.
        
    4.  Set the **Name** to **Temporary Holding**.
        
    5.  Click **Save**.
        
2.  Write a check:
    
    1.  Go to _Transactions > Bank > Write Checks_.
        
    2.  In the **Payee** field, select your vendor.
        
    3.  On the **Expenses** subtab, in the **Account** column, select your **Temporary Holding** account.
        
    4.  In the **Amount** column, enter the prepayment amount.
        
    5.  Optionally include notes in the **Memo** column for the purpose of this prepayment.
        
    6.  Click **Add**.
        
    7.  Click **Save**.
        
3.  Enter a vendor credit:
    
    1.  Go to _Transactions > Payables > Enter Vendor Credits_.
        
    2.  Select your vendor.
        
    3.  On the **Expense** subtab, select your **Temporary Holding** account.
        
    4.  In the **Amount** column, enter the prepayment amount.
        
    5.  Click **Add**.
        
    6.  Click **Save**.
        

These two transactions should do the following:

-   Enable you to pay the vendor in advance.
    
-   Update your holding account so the resulting balance is zero.
    
-   List an outstanding vendor credit on the vendor's account.
    

When you receive the vendor's bill, you can apply this credit.

### Related Topics:

-   [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html)
-   [Writing Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1543875.html)
-   [Entering Vendor Credits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2392083.html)

### How do I import sales tax tables? {#question_N3908817}

The Use State Sales Tax Tables feature enables you to update existing tax tables and to add state taxes which were not initially set up.

#### To update existing sales tax tables: {#procedure_N3908830}

1.  Go to _Setup > Accounting > Taxes > Use State Sales Tax Tables_.
    
2.  Choose the state you are updating in the **State** field.
    
3.  Make sure that each tax type has a tax agency and a tax control account specified.
    
    You can create:
    
    -   Tax Types at _Setup > Accounting > Taxes > Tax Types_.
        
    -   Tax Agencies at _Lists > Relationships > Vendors_.
        
        Make sure to select a vendor category that has the **Tax Agency box** marked.
        
    -   Tax Accounts at _Setup > Accounting > Taxes > Tax Control Accounts_.
        
4.  Click **Save**.
    

You can now view the tax rates by navigating to _Setup > Accounting > Taxes > Tax Codes_. Then, click Tax Groups or Tax Codes. Changes to tax rates do not have a retroactive effect on transactions. All changes effect only future transactions.

#### To add state taxes which were not initially set up or made available for import: {#procedure_N3908903}

1.  If you use the **Advanced Taxes** feature, go to _Setup > Accounting > Taxes > Set Up Taxes_.
    
2.  Click **Add New State**.
    
3.  In the popup window, select which **State** you setting up.
    
4.  Enter a **Description** for the state.
    
5.  Click **Save**.
    

Now go to _Setup > Accounting > Taxes > Use State Sales Tax Tables_.

1.  Select our newly created state in the **State** dropdown list.
    
2.  Make sure that each tax type has a tax agency and a tax control account specified.
    
    You can create:
    
    -   Tax Types at _Setup > Accounting > Taxes > Tax Types_.
        
    -   Tax Agencies at _Lists > Relationships > Vendors_.
        
        Make sure to select a vendor category that has the Tax Agency box marked.
        
    -   Tax Accounts at _Setup > Accounting > Taxes > Tax Control Accounts_.
        
3.  Click **Save**.
    

### Related Topics:

-   [Setting U.S. Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2038835.html)
-   [Creating Tax Codes - U.S. Nexus](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2039577.html)

### Does changing a general ledger account on an item record affect previous transactions? {#question_N3909065}

Changes to the general ledger account selected on item records can affect historical transactions.

When you change an account assigned on an inventory record, the new account is used not only for future transactions, but is also retroactive, and historical transactions are updated to reflect the new account. You cannot use one account for an item on past transactions and a different account on new transactions.

Important:

Variance accounts are expense accounts. If you change a variance account on an item record, it affects the general ledger impact only for future transactions created after you save the change. Changing a variance account on an item record does not affect historical transactions. To update the general ledger impact of a historical transaction, you must edit the actual transaction record.

When you edit an item record and save changes that include an account change, you receive this warning:

You have changed the account(s) for this item. Click OK to update the accounts on existing transactions or Cancel to stay on this page.

You can do one of the following:

-   Click **OK** to save the item record including the account change and to use the new account on historical transactions AND future transactions.
    
-   Click **Cancel** to save the item record without changing the account, and to continue using the original account on historical transactions and future transactions.
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
