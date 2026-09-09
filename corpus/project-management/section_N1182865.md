---
id: "section_N1182865"
type: "section"
title: "Working with Project Management in OneWorld"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Using Project Management > Working with Project Management in OneWorld"
parent: "chapter_N1179876"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1182865.html"
anchors: ["subsect_164311099534", "subsect_162090033221", "subsect_162090210296", "subsect_162090214477"]
sha256: "c7fd36d844af4c603cb2b76e9b9578dff5b9d58bdbbe8c676864839416a9ba3b"
---

When you create a project record and link it to a customer, the project automatically uses the customer's subsidiary, and that can't be changed.

If you create a project that isn't linked to a customer, there's no subsidiary by default, so you'll need to select one. After you enter transactions associated with the project, the project subsidiary can't be changed unless the transactions are deleted.

Sub-projects are associated with the subsidiary of the parent project.

You can assign any employee to any project regardless of their subsidiary. For example, an engineer associated with Wolfe US can be assigned as a resource for a project associated with Wolfe UK.

Only resources associated with the project's subsidiary can enter billable time and expenses against the project.

Note:

To allow resources to enter time and expenses for customers of subsidiaries other than their own, you must enable the Intercompany Time and Expense feature. An automated adjustment process is available to transfer charges for intercompany expenses from the employee subsidiary to the customer subsidiary. See [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html).

## Project Intercompany Cross Charge Request {#subsect_164311099534}

Project Intercompany Cross Charge Request is a part of the [Intercompany Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_158142795285.html). This feature lets you cross-charge amounts between subsidiaries with the integration period end process. You can set amounts in a currency to be used for intercompany cross-charging reflected in Intercompany Cross Charges.

### Creating Project Intercompany Cross Charge Request {#subsect_162090033221}

#### To create a project intercompany cross charge request:

1.  Go to _Transactions > Financial > Create Project Intercompany Cross Charge Requests_.
    
2.  Select your project.
    
    Note:
    
    The selling subsidiary pre-fills automatically in the **From Subsidiary** field based on your selected project.
    
3.  Select a buying subsidiary from the list.
    
4.  Select the amount, currency and trigger.
    
    You can choose between date, project completion and project tasks/milestone completion triggers.
    
    -   Date - a date when you want the transaction to happen.
        
    -   Project Completion - select if you want a project completion as a trigger.
        
    -   Project Tasks/Milestone Completion - allows you to select a project task from the list of your tasks to apply the request.
        
5.  Click **Save**.
    

### Creating a copy of the Project Intercompany Cross Charge Request {#subsect_162090210296}

You can create a copy of the project intercompany cross charge requests.

#### To create a copy of the project intercompany cross charge requests:

1.  Go to _Transactions > Financial > Create Project Intercompany Cross Charge Requests_.
    
2.  Select your project.
    
3.  Click **Actions**.
    
4.  Click **Make Copy**.
    

### Creating Project Intercompany Journal Entries {#subsect_162090214477}

You can create journal entries for project intercompany cross charge requests.

#### To create journal entries:

1.  Go to _Transactions > Financial > Make Intercompany Journal Entries_.
    
2.  Select the Cross Charge Journal filter type.
    
3.  Select your project.
    
4.  Fill out the fields at the top of the form.
    

Note:

All amounts are auto-calculated to EUR.

For more information, see [Making Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469880.html) and [Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1468455.html).

You might have to set up the relationship between your chosen subsidiaries by managing intercompany cross charges. Be sure to follow any instructions in the error message in Transactions > Financial > Manage Intercompany Cross Charges > Error message. Examples below:

#### Managing Project Intercompany Cross Charges

1.  Go to _Transactions > Financial >Manage Intercompany Cross Charges_.
    
2.  Click Message Log and act according to the error message displayed.
    
3.  Click **Set Up** on the **Recommended Action** subtab of the message log.
    
    1.  For example: If the error message states that it can't find the representing entities, click the **Representing Entities** subtab.
        
    2.  Click the **Subsidiaries** page link.
        
        A new window with the list of subsidiaries open.
        
    3.  Click **Subsidiary Settings Manager** at the top right of the page.
        
        This step enables you to set up the subsidiary.
        

#### Creating a new Customer Entity

1.  Go to _Lists > Relationships > Customers > New_
    
2.  Enter required fields such as client name, status and custom form.
    
    Select the initial subsidiary in the **Represents Subsidiary** field.
    
3.  Go to the **General** subtab and select the final subsidiary in the **Subsidiary** field.
    
4.  Go to the **Financial** subtab and select the currency in the Currencies > Currency.
    
    Warning:
    
    Select the same currency as in the intercompany framework, and in the error message.
    

#### Creating a new Vendor Entity

1.  Go to _Lists > Relationships > Vendors > New_.
    
2.  Enter required fields.
    
    Select the initial subsidiary.
    
3.  Go to the **Company profile** subtab and select the final subsidiary.
    

### Related Topics:

-   [Using Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1179876.html)
-   [Project Management Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1182526.html)
-   [Creating a Project Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1183012.html)
-   [Associate Subsidiaries with Entities and Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276477.html)
-   [Set up NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268052.html)
-   [Representing Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159067444188.html)
-   [Best Practices for Using the Intercompany Framework Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1522434159.html)
-   [Requirements for the Intercompany Framework Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1522768517.html)
-   [Intercompany Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1549982657.html)
-   [Intercompany Cross Charges](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519995046.html)
-   [Intercompany Netting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_158945626309.html)
-   [Intercompany Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_158142795285.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
