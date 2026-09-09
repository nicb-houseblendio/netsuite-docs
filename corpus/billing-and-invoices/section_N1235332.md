---
id: "section_N1235332"
type: "section"
title: "Custom Workflow Based Invoice Approval"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Invoices > Custom Workflow Based Invoice Approval"
parent: "section_N1235134"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1235332.html"
anchors: []
sha256: "3ccc4e2719f945f80b882771d29f470fb9201a0a50505007ac0c66d0e935da89"
---

You can create a custom workflow or use the standard workflow for invoice approvals. A custom workflow gives you the most flexibility for processing approvals. For more information, read [Using Custom SuiteFlow Workflows for Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396465.html).

You can use SuiteFlow to create your own custom workflow to process invoice approvals.

-   To use SuiteFlow to create a custom workflow for invoice approvals, enable approval routing for invoices first. To enable approval routing for invoices, go to _Setup > Accounting > Accounting Preferences_. On the **Approval Routing** subtab, check the **Invoices** box. For more information about approval routing, read [Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2394992.html).
    
-   To create workflows using SuiteFlow, enable SuiteFlow by going to _Setup > Company > Setup Tasks > Enable Features_. Click the **SuiteCloud** tab, and then check the **SuiteFlow** box. Click **Save**.
    

For workflow based invoice approvals, you can create a custom workflow.

Consider adding these options in your custom invoice approval workflow:

-   Hierarchical or custom routing rules
    
-   Email notifications that include links to drill down to records for approval
    
-   Approve and Reject buttons
    
-   Respecting approval limits
    
-   Updating the **Approval Status** and **Next Approver** fields on records
    
-   Preventing pending approval records from being edited
    
-   Designating an alternate approver.
    

#### To complete a basic invoice approvals workflow:

1.  Go to Customization > Scripting > Workflows > New (Administrator).
    
2.  Under Basic Information:
    
    -   In the **Name** field, enter **Invoice Approval**
        
    -   In the **Record Type** field, select **Transaction**
        
    -   In the **Sub-Types** field, select **Invoice**
        
    -   In the **Release Status** field, select **Released**
        
3.  Under Event Definition:
    
    -   Check the **On Create** box
        
    -   In the **Context** field, select **CSV Import** and use Ctrl+click to also select **User Interface**
        
4.  Click **Save**.
    
5.  Double-click **State 1** to open the Workflow State page.
    
6.  In the **Name** field, enter **Pending Approval**, and then click **Save**.
    
7.  In the bottom, right side of the page, click **New Action**.
    
8.  Click **Set Field Value**.
    
9.  On the Workflow Action page:
    
    -   Under Parameters, in the **Field** field, select **Approval Status**
        
    -   Under Value, select **Static Value**
        
    -   In the **Selection** field, click the double arrows, select **List**, and then select **Pending Approval**
        
    -   Click **Save**
        
10.  Click **New Action**.
     
11.  Click **Add Button**.
     
12.  In the **Event Type** field, select **View**.
     
13.  In the Parameters section, enter **Approve** in the **Label** field.
     
14.  Click **Save**.
     
15.  In the Workspace, click **New State**.
     
16.  Double-click **New State** to open the Workflow State page.
     
17.  In the **Name** field, enter **Approved**, and then click **Save**.
     
18.  In the Diagram frame, click **Approved**.
     
19.  Click the **Actions** subtab, and then click **New Action**.
     
20.  Click **Set Field Value**.
     
21.  Under Parameters, select **Approval Status** in the **Field** field.
     
22.  Under Value:
     
     -   Select **Static Value**
         
     -   In the **Selection** field, click the double arrows, select **List**, and then select **Approved**
         
23.  Click **Save**.
     
24.  Click the icon at the bottom of the **Pending Approval** state then drag the arrow to create a transition to the **Approved** state.
     
25.  Double-click the arrow to open the Transition window and edit the workflow transition properties as needed.
     

Note:

If you use SuiteFlow for invoice approval, all invoices start with Pending Approval status by default.

You can always manually set an invoice to Approved for basic approvals.

Note:

The SuiteFlow conditions used for Bulk Approvals for records using custom approvals have been updated for the invoice record. Prior to 2016.2, both the workflow button's condition and the Next Approver condition filtered invoice records for bulk approvals. The Next Approver condition checks that the **Next Approver** field on the record has the current logged-in user. Beginning in 2016.2, the Next Approver condition is no longer used to filter records for bulk approvals for this record. Records are now filtered for bulk approvals using only the workflow button's condition. If you want to continue filtering records based on the **Next Approver** field, add the condition to the workflow button. If you need help, contact Customer Support.

### Related Topics

-   [Transactional Impact for Workflow Based Invoice Approvals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4025082250.html)
-   [Custom Workflow Based Invoice Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1235332.html)
-   [Global Invoicing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1237960.html)
-   [Creating an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1238506.html)
-   [Payment Date Prediction for Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0106021633.html)
-   [Choosing an Invoice Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240040.html)
-   [Billing Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4063198073.html)
-   [Billing or Invoicing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240951.html)
-   [Invoicing Billable Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1241287.html)
-   [Closing or Voiding an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158654862294.html)
-   [Creating Installments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540928779.html)
-   [Printing an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1242104.html)
-   [Progress Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1243687.html)
-   [Billing Costs to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248576.html)
-   [Displaying Deposit Balance on Customer Statements and Remittance Slips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4204723346.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
