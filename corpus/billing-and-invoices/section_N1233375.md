---
id: "section_N1233375"
type: "section"
title: "Using Billing Classes"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Billing > Using Billing Classes"
parent: "chapter_4419712298"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233375.html"
anchors: ["bridgehead_N1233506"]
sha256: "e669db99ea700aaaeb312579a1ece87562cf91f32fa4bd925e27356571ef14ab"
---

You can use billing classes to set billable time rates for service items based on employees.

When different employees charge different rates for the same service, create billing classes and assign a billing class to employees. Set the pricing for each billing class on service item records. Then, the correct default pricing shows when an employee enters billable time to invoice the customer.

You can create a billing classes for individual employees or groups, and charge a different rate for each.

For example, a law office can use billing classes to charge specific hourly rates for time billed by partners in the firm:

For example, you run a law firm and create two billing classes called Junior Partner and Senior Partner. You associate the Junior Partner and Senior Partner billing classes with the service item Initial Consultation and set the appropriate billing rates for each. Also, you select the Junior Partner billing class on John Smith's employee record. Then, when John Smith enters billable time for an initial consultation, the time is billed at the junior partner rate by default.

Using Billing Classes requires the four following steps:

1.  [Enable the Bill Costs to Customers feature](#bridgehead_N1233506)
    
2.  [Creating Billing Classes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233628.html)
    
3.  [Specify Billing Classes on Employee Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233628.html#bridgehead_N1233694)
    
4.  [Track Billing Class Pricing on Service Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233628.html#bridgehead_N1233772)
    

#### Enable the Bill Costs to Customers feature {#bridgehead_N1233506}

1.  Go to _Setup > Company > Enable Features_ (Administrator).
    
2.  Click the **Transactions** subtab and check the **Bill Costs to Customers** box under Billing.
    
3.  Click the **Employees** subtab and under Time & Expenses, check the **Time Tracking** box .
    
4.  Check the **Per-Employee Billing Rates** box.
    
5.  Click **Save**.
    

Now that these features are enabled, you can create billing classes. Create a billing class for each category you want to create prices for.

### Related Topics

-   [Billing and Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1232486.html)
-   [Creating Billing Classes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233628.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
