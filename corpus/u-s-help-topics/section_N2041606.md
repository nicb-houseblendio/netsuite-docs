---
id: "section_N2041606"
type: "section"
title: "Enabling U.S. Tax Lookup"
branch: "u-s-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > U.S. Help Topics > Taxation Features For Accounts without SuiteTax > Enabling U.S. Tax Lookup"
parent: "section_156940239941"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2041606.html"
anchors: []
sha256: "d9364832208ebb279687017a5ddb772c2e965fdef2aba4ed685c91465e7a082e"
---

If you enable Tax Lookup on Sales Transactions, NetSuite can determine the proper tax code automatically when an order is entered manually or through your website.

#### To enable U.S. tax lookup:

1.  Go to _Setup > Accounting > Taxes > Set Up Taxes_.
    
2.  Check the **Enable Tax Lookup on Sales Transactions** box
    
3.  click **Save**.
    

With tax lookup enabled, NetSuite determines the appropriate tax group or tax code for a customer based on the customer's shipping address.

When customers enter orders on your web store, the tax group corresponding with the customer's shipping address is applied to the order. Also, when a transaction is entered manually for a customer, the tax group that corresponds to the customer's shipping address is selected by default.

NetSuite compares the state and zip code on the customer's shipping address to existing tax codes or groups in the following situations:

-   No tax code is selected on the customer's record
    
-   The state in the customer's shipping address does not match yours
    

After comparing, if the system can't find a tax code, then no tax is charged on the transaction.

You can choose to automatically select tax codes based on customer addresses by going to _Setup > Accounting > Taxes > Set Up Taxes_. On the United States subtab:

-   If you check the **Charge Out of District Sales Taxes** box, NetSuite searches for tax codes or groups that match the customer's shipping address. Only the tax codes for nexuses assigned to the subsidiary will be available in transactions. A sales transaction isn't taxable if the nexus isn't assigned to the subsidiary, even if the customer is taxable or the item is taxable in the customer's state.
    
-   If you don't check the **Charge Out of District Sales Taxes** box, and there is no default tax item set on the customer record, then the system uses the home tax code for the corresponding state. If there is no home tax code, then the system uses the default tax code for the United States.
    

Important:

In NetSuite U.S. edition accounts without Advanced Taxes, a customer isn't taxable only if the **Taxable** box isn't checked and the **Tax Item** field is blank on the customer record. Previously, on the customer record, if the **Tax Item** field has a value, the system ignores it if the **Taxable** box isn't checked. Similarly, the system ignores any tax codes or tax schedules selected on the item record or transaction record for that customer. In Version 2012, Release 2, a change in the tax lookup for U.S. edition NetSuite accounts removed the values in the **Tax Item** field on customer records in which the Taxable box isn't checked. If you are using the **Tax Item** field for purposes other than tax lookup, manually set the **Tax Item** field back to its original value. If **Tax Item** field has a value, the tax lookup returns that value instead of **not taxable** even if the **Taxable** box isn't checked. For example, you can set the **Tax Item** field to Avalara even if the **Taxable** box isn't checked.

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html)
-   [Setting U.S. Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2038835.html)
-   [Creating Tax Codes - U.S. Nexus](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2039577.html)
-   [Paying Sales Tax - United States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2041996.html)
-   [U.S. Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2042330.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
