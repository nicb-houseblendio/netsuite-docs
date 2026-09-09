---
id: "section_N2578016"
type: "section"
title: "Customizing the Website Registration Form"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Setting Up Your Site Builder Site > Customizing Registration for Your Site Builder Web Store > Customizing the Website Registration Form"
parent: "section_N2576937"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2578016.html"
anchors: ["procedure_N2578066"]
sha256: "d9cc690afd5aa224f3e39bd8661f0b360a954026a798e87c500de2c19bf48c5a"
---

You can use custom entity fields in your website to collect additional information from your customers during registration. When shoppers register, the information they enter shows up in the customer record created in NetSuite. Employees with the Store Manager role cannot set up custom entity fields. These steps are provided for those with Administrator roles.

#### To use entity fields in your site: {#procedure_N2578066}

1.  Go to _Customization > Lists, Records, & Fields > Entity Fields > New._.
    
2.  In the **Label** field, enter a name for the custom field.
    
3.  In the **ID** field, enter an ID for this field with no spaces.
    
    This ID is used in attribute tags if you want to call information saved in this field for display in your site. For more information, see [Creating Attribute Tags for Custom Records and Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616759.html).
    
4.  Select a kind of custom field in the **Type** field.
    
5.  If you selected List/Record in the Type field, select the type of list or record that can be selected in this field.
    
6.  Make sure the **Store Value** box is checked to store the information gathered in this field in your account. You should only clear this box if this field is meant for display only.
    
7.  Check the **Show In List** box to show information from this field on entity lists.
    
8.  If you selected List/Record in the Type field, you can check the **Record is Parent** box to indicate that the record type selected is a parent record. This field is used to create a parent-child relationship between two record types.
    
9.  On the **Applies to** subtab, check the **Customer, Project** and **Web Site** boxes. Checking these two boxes indicates for your custom field to appear in both your site registration form and in customer records.
    
10.  On the **Display** subtab, set the display location and enter help for this field.
     
11.  On the **Validation & Defaulting** subtab, decide if you want to make this field mandatory for customers or to check spelling in the field.
     
12.  On the **Sourcing & Filtering** subtab, decide what should be available for selection in this field. Selections available for sourcing depend on the type of custom field you are creating.
     
13.  Click **Save**.
     

This custom entity field appears in the registration of your site. When a customer registers in your site, these custom entity fields automatically record your customer's information on their customer record.

### Related Topics

-   [Secure Login Access to Your NetSuite Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577046.html)
-   [Displaying Login Fields on Your Web Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577156.html)
-   [Customizing Login and Logout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577359.html)
-   [Registration-Free Shopping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577575.html)
-   [Restricting Access to Your Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577753.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
