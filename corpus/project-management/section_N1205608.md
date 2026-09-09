---
id: "section_N1205608"
type: "section"
title: "Project Billing Rates"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Project Billing > Project Billing Rates"
parent: "section_N1204906"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205608.html"
anchors: []
sha256: "c46c53f311163ae3f56a5ec7677c2c086efc10fa72827cfc4c3a4b72835a69e0"
---

You specify the billing rates for a project when you assign resources to the project's tasks. The employee's price rate fills in by default, but you can change it if needed. If you update the default rate on an employee record, NetSuite updates the rate on the project as well.

You can define pricing for service items in the following ways:

-   **Use Service Item Price**
    
    This is the simplest form of billing. The price per unit of time comes from the service item linked to the project task assignment line.
    
    -   Price Level
        
        The price level for the associated customer determines the default price for the service item if you assign a customer before saving the project.
        
        If you assign a customer to a project after saving it, then the base price for the service item is used.
        
    -   Quantity Pricing
        
        If quantity pricing is enabled, then quantity-based discounts are enabled on a line-by-line basis.
        
    
    For example, if there's special pricing for 10+ units, it only applies if a single task line has more than 10 units. If the work is split among several resources, the discount doesn't apply.
    
-   **Use Per-Employee Rates**
    
    When per-employee rates are enabled, you can use billing classes with projects. Billing classes let you set up different roles, such as Consultant, Analyst, or Project Manager, and create different rates for each role, depending on what service or item is being offered.
    
    You can assign each employee a default class in the Classification section of the employee record. You can also assign a default billing class to vendors that serve as project resources on the Financial tab of the vendor record. When you assign a resource with a billing class to a project task, the price for that resource is calculated from the billing class price.
    
    Billing classes can also be assigned to service items for sale and resale. When you assign a billing class to an item, you can define a different price structure that applies only to that service item. When you use a service item on a project task, the price is calculated based on the service item billing class and will override the default resource billing class price.
    
    If you use billing classes, you can also enable Billing Rate Cards to define different rates for a group of billing classes. You can then assign these rate cards to customers and use them as the basis for time-based charge rules on charge-based billing projects.
    
-   **Customize Price on Project Task**
    
    Customize the default pricing that is sourced on the task line regardless of any other pricing provided.
    

When you enter time against a project and select a task, then the billing rate is sourced from the rate on the project task. Since the basic pricing is the same for project tasks and regular billable time entry, this number is usually the same, unless you've manually customized the task pricing.

### Related Topics

-   [Project Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204906.html)
-   [Projects and Time and Materials Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205953.html)
-   [Projects and Interval Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1206277.html)
-   [Projects and Milestone Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1206555.html)
-   [Project Management Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1207852.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
