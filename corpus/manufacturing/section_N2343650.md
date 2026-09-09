---
id: "section_N2343650"
type: "section"
title: "Defining a Manufacturing Charge Item"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Routing > Setting Up Manufacturing Routing > Defining a Manufacturing Charge Item"
parent: "section_N2341463"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2343650.html"
anchors: ["procedure_N2343677"]
sha256: "296f2e3516b1290fe2abca5b1ad51941915eedf854ff129ff77b4e0ed4543031"
---

With Manufacturing Routing and Work Center, when a specific routing operation is recorded, you can use items to define charges for the activity. For example, you can define the hourly cost of activities being performed, and the expense account the charges are logged against. To do so, you must set up the item record to define the item as a manufacturing charge item.

#### To define an item as a manufacturing charge item: {#procedure_N2343677}

1.  Go to _Lists > Accounting > Items > New_.
    
2.  Click a link to create a charge item. You can track routing charges and expenses using the following item types:
    
    -   Other Charge (for Purchase or for Resale)
        
    -   Service (for Purchase or for Resale)
        
3.  Enter an **Item Name**.
    
    For example, Machine Run Time Cost.
    
4.  If you use NetSuite OneWorld, select a **Subsidiary**.
    
    A manufacturing charge item can be associated with only one subsidiary.
    
5.  On the item record, check the **Manufacturing Charge Item** box.
    
    This box cannot be cleared if the item is included in a cost template.
    
    You cannot check the **Include Children** box on the item record when the **Manufacturing Charge Item** box is checked.
    
6.  Select a **Cost Category**.
    
    The cost category cannot be changed if the manufacturing charge item is included in a cost template.
    
    Only manufacturing charge items can use the labor and machine cost categories.
    
7.  Enter an hourly rate up to 7 decimal places in the **Purchase Price** field.
    
    Charges are based on hourly rate (amount per hour).
    
8.  Click the **Accounting** subtab.
    
9.  Select the expense account these hourly charges should be logged against.
    
10.  Complete any additional necessary fields.
     
11.  Click **Save**.
     

A manufacturing charge item cannot be associated with a unit type even if you use the Multiple Units of Measure feature. For information, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).

Important:

The currency for manufacturing charge items is derived from the item record and defaults to the parent subsidiary's base currency. To use a different currency, set a preferred vendor with the appropriate currency on items used in routings.

### Related Topics

-   [Setting Up Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2341463.html)
-   [Enabling the Manufacturing Routing Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2341773.html)
-   [Setting Routing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3950900044.html)
-   [Defining Cost Categories for Manufacturing Routing and Work Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2342063.html)
-   [Creating Manufacturing Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2344013.html)
-   [Creating Manufacturing Work Centers or Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2344727.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
