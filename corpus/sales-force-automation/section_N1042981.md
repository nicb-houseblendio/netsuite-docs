---
id: "section_N1042981"
type: "section"
title: "Reassigning Customers to Sales Territories"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Setting Up SFA > Reassigning Customers to Sales Territories"
parent: "chapter_N1035717"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1042981.html"
anchors: ["procedure_N1043010"]
sha256: "d0d83d5f2fa59fea6689e4121135c22a931ad479fa97fe2e46d537859007deb4"
---

You can reassign existing customers, prospects, or leads based on your current sales rules and territories. Reassigning customers is useful when you restructure your sales territories, or when customers move.

**Example: Reassigning Customers Based on Relative Account Size**

Wolfe Electronics wants to reassign sales reps in the state of California based on the size of their customers' businesses. They use the Credit Limit field (on Financial subtab of the customer record) to measure account size. They create a new sales rule and sales territory called Key Accounts. They assign customers with a credit limit over $500,000 to the Sales Director and then perform a mass update that limits the customer record set to California.

#### To reassign customers to new sales territories: {#procedure_N1043010}

1.  Create your revised sales rules and territories.
    
    See [Sales Rules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1039705.html) and [Setting Up a Sales Territory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1042578.html).
    
2.  Go to _Lists > Mass Update > Mass Updates_.
    
3.  Click **Sales Force Automation** to expand the SFA mass update options.
    
4.  Click **Reassign Customers by Sales Territory Rules**.
    
5.  Define your search criteria to filter which customers you want to reassign based on current sales rules and territories.
    
    In the example above, you'd filter the results by State/Province > any of > California.
    
6.  Click **Preview**.
    
7.  Clear the box in the **Apply** column next to customers you don't want to reassign.
    
8.  Click **Perform Update**. NetSuite shows a popup window notifying you that the mass update is in progress. You can monitor the progress of the mass update by clicking **Refresh**.
    

Note:

You can perform only one mass update at a time.

### Related Topics

-   [Customer Statuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1036969.html)
-   [Sales Territories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1040011.html)
-   [Team Selling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1037318.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
