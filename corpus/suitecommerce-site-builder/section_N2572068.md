---
id: "section_N2572068"
type: "section"
title: "Customizing Checkout in Site Builder"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Setting Up Your Site Builder Site > Customizing Checkout in Site Builder"
parent: "chapter_N2576231"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2572068.html"
anchors: ["procedure_N2572112"]
sha256: "72e2eb0e72dd5e2e075b2218efb0bfc0ed7ae5e8bdda67364a341d56d8c94ef3"
---

Use custom transaction body fields in your web store to collect additional information from your customers during checkout.

When shoppers check out, the information they enter shows up on the sales order created in NetSuite.

#### To use transaction body fields in your store: {#procedure_N2572112}

1.  Go to _Customization > Lists, Records, & Fields > Transaction Body Fields > New._.
    
2.  In the **Label** field, enter a name for the custom field. This is the name of the field as it will show to customers.
    
3.  In the **ID** field, enter an ID for this field with no spaces. This ID is used in attribute tags if you want to call information saved in this field for display in your site. For more information, see [Creating Attribute Tags for Custom Records and Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616759.html).
    
4.  Select an option in the **Type** field.
    
5.  If you selected List/Record in the Type field, select the type of list or record that can be selected in this field.
    
6.  Make sure the **Store Value** box is checked to store the information gathered in this field in your account. You should only clear this box if this field is meant for display only.
    
7.  Check the **Show In List** box to show information from this field on sales transactions lists.
    
8.  If you selected List/Record in the Type field, you can check the **Record is Parent** box to indicate that the record type selected is a parent record. This field is used to create a parent-child relationship between two record types.
    
9.  On the **Applies to** subtab, check the **Sale** and **Web Store** boxes. Checking these two boxes indicates for your custom field to appear in both your store and on sales orders.
    
10.  To print this custom field on standard forms, check the **Print on Standard Forms** box.
     
11.  On the **Display** subtab, set display location and enter help for this field
     
12.  Click the **Validation & Defaulting** subtab, and then check the **Mandatory** box to make this a required field. This subtab also includes other options such as **Maximum Length**, and **Default Value**.
     
13.  On the **Sourcing & Filtering** subtab, decide what options customers should be able to select online. Selections available for sourcing depend on the type of custom field you are creating.
     
14.  Click **Save**.
     

This custom body field appears in the checkout of your store. When you approve a sales order from your store, these custom body fields automatically record your customer's information on the sales order.

### Related Topics

-   [Site Builder Web Site Content Manager](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2576424.html)
-   [Customizing the Shopping Cart in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2571864.html)
-   [Best Practices for Website Performance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2461527.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
