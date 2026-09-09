---
id: "section_N1233628"
type: "section"
title: "Creating Billing Classes"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Billing > Using Billing Classes > Creating Billing Classes"
parent: "section_N1233375"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233628.html"
anchors: ["bridgehead_N1233694", "bridgehead_N1233772"]
sha256: "de90c60c0582bece13373376e9b0a77a4a8ea2db9ae9260ac7a8db703646b545"
---

1.  Go to _Setup > Accounting > Billing Classes > New_.
    
2.  On the Billing Class page, enter the name of the billing class.
    
    For example, enter Junior Partner or Senior Partner.
    
3.  If you're using Multiple Units of Measure and Charge-Based Billing, you can select a Price, Units Type, and Sale Unit to use custom interval billing rates. For more information, see [Custom Interval Billing Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4369706980.html#bridgehead_4526273368).
    
4.  Click Save.
    

After you've created billing classes, they appear in the billing class lists on service item records and employee records.

Note:

If you're using Project Management and Charge-Based Billing for projects, you can also enable billing rate cards to define different billing rates for groups of billing classes. You can then use these rate cards to set billing rates on charge-based projects using time-based charge rules. For more information, see [Using Billing Rate Cards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4689764278.html).

If you're using rate cards, billing class records won't have a field for defining rates. You must define rates for billing classes used for projects on billing rate cards. After you enable the feature, a default billing rate card is automatically created with your existing billing classes and default rates.

Next, you can select the default billing class to determine the rate billed for each employee.

#### Specify Billing Classes on Employee Records {#bridgehead_N1233694}

1.  Go to _Lists > Employees > Employees_.
    
2.  Click **Edit** next to an employee.
    
3.  Under Classification, in the **Billing Class** field, choose a billing class.
    
4.  Click **Save**.
    

Now, when billable time is entered in Time Tracking for this employee, the default rate charged is the rate set for the billing class on the service item record.

On service item records, enter rates for each billing class to set pricing.

#### Track Billing Class Pricing on Service Items {#bridgehead_N1233772}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click **Edit** next to a service item. The item type must be Service for Sale or Service for Resale.
    
3.  On the item record, click the **Sales/Pricing** subtab.
    
4.  Under Sales, select a billing class.
    
    For example, select Senior Partner to set up senior partner rates.
    
5.  Under Pricing, make sure you've entered default prices on your base currency subtab.
    
6.  Enter the appropriate pricing for that billing class.
    
    Billing classes can't have negative rates.
    
7.  Click **Add**.
    
8.  Set additional billing classes and rates as needed.
    
9.  Click **Save**.
    

When you enter the service item in Time Tracking for an employee with a billing schedule, the correct pricing shows up automatically.

For more information about invoicing customers for billable time, read [Billing Time to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1249803.html).

Note:

Because the Billing Classes feature is not compatible with the Quantity Pricing feature, you can't use both features at the same time. If both are enabled, then billing classes replace quantity pricing on service item records.

### Related Topics

-   [Deciding Between Invoices and Cash Sales](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233061.html)
-   [Statement Charges](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233128.html)
-   [Adding Billing Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588267772.html)
-   [Using Consolidated Billing for Projects and for Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233909.html)
-   [Creating Terms of Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234186.html)
-   [Using Terms of Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234578.html)
-   [Remittance Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234795.html)
-   [Printing Remittance Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234980.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
