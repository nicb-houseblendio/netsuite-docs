---
id: "section_N1085616"
type: "section"
title: "Creating a Subcustomer Record"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Record Management > Customers > Creating a Subcustomer Record"
parent: "section_N1076428"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1085616.html"
anchors: ["procedure_N1085748"]
sha256: "2069ab44b1524ecb9a7239737ee3371b06d40ba617fa23fcefd216a8d1e47fa9"
---

A subcustomer record is a customer record that has another customer record as its parent. Subcustomer records let you create hierarchies of leads, prospects, or customers to organize and manage relationships between your employees and your customers.

Subcustomer records have the same fields and functionality as customer records. In a subcustomer record, the Parent Company has a value. Your customer for a sales transaction can be a subcustomer, and subcustomers can have their own subcustomers and projects.

The credit limit you set for a customer doesn't include any of the customer's subcustomers. The customer may reach its credit limit, but you can continue to create sales transactions for its subcustomers without restrictions. For more information, see [Managing Customer Credit Limits and Holds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1080144.html).

Reports that show customers, prospects, and leads also show subcustomers. Subcustomer records appear indented under the parent customer.

In NetSuite OneWorld, you can use subcustomer records for a customer that does business with more than one of your company's subsidiaries. Subcustomers can be assigned a subsidiary different than that of the parent subsidiary. For more information, see [Associate Subsidiaries with Entities and Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276477.html).

Note:

Projects are tracked as subcustomers unless the Advanced Project Tracking feature is enabled. For more information, read [Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3714107248.html).

NetSuite limits the maximum number of customers you can have in a customer-subcustomer hierarchy. A customer hierarchy is comprised of the top-level parent customer, all of its subcustomers, and all of their subcustomers. You can have a maximum of 10,000 customers and subcustomers in a customer hierarchy.

If you need to increase the limit for your account, contact Customer Support. Exceeding the hierarchy limit may impact performance related to customer credit limits, customer balances, consolidated balances, and payments.

#### To create a subcustomer record: {#procedure_N1085748}

1.  Go to _Lists > Relationships > Customers_.
    
2.  Click **View** next to the name of the lead, prospect, or customer for which you want to create a subcustomer.
    
3.  From the **Create New** menu, select **New Subcustomer**.
    
    The subcustomer record is the same as a customer record except that
    
4.  In the **Company Name** or **Name** fields, enter your new subcustomer's name.
    
    The **Parent Company** field automatically shows the name of the customer from which you created the subcustomer record.
    
5.  In the **Status** field, select the appropriate status.
    
6.  NetSuite OneWorld: If this subcustomer is associated with a different subsidiary than the parent customer, select the appropriate **Subsidiary**.
    
7.  Complete the subtabs as appropriate.
    
    When you create a subcustomer record, the customer contacts aren't copied to the new subcustomer record.
    
    For information, see [Customer Record Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_161887259374.html).
    
8.  Click **Save**.
    

### Related Topics

-   [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html)
-   [Creating a Customer Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161860867711.html)
-   [Viewing Recent Customer Activity](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161945846485.html)
-   [Merging Customer Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509542900.html)
-   [Attaching Events, Tasks, and Calls to Records and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1084924.html)
-   [Inactivating or Deleting Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515598204.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
