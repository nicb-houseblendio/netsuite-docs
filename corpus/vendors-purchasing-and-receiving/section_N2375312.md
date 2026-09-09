---
id: "section_N2375312"
type: "section"
title: "Standard Vendor Bill Approval FAQ"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Bills > Vendor Bill Approvals > Standard Vendor Bill Approval FAQ"
parent: "section_N2373552"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2375312.html"
anchors: ["question_N2375325", "question_N2375374", "question_N2375396", "question_N2375449", "question_N2375470", "question_N2375492", "question_N2375545", "question_N2375616", "question_N2375637"]
sha256: "9c5a8cbab919ff790acffce85ed72270a639d71d47086f824476a6879377c62c"
---

### Where can I set the default approval status of vendor bills? {#question_N2375325}

In the Default Vendor Bill Status field. See [Setting the Default Vendor Approval Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2374176.html).

### If a Vendor Bill is accidentally approved, can a vendor bill with an Approved status be changed back to Pending Approval? {#question_N2375374}

Not through the user interface. You will have to delete the bill and recreate it. If you approve vendor bills through a script or workflow, you can change it back to Pending Approval.

### Is there a way to mass approve vendor bills? {#question_N2375396}

Yes. Use the Approve Bills page.

See [Bulk Approving Vendor Bills With Standard Vendor Bill Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2374794.html).

### Is there an approval history on a vendor bill? {#question_N2375449}

The approval history can be found on the System Notes subtab of the bill.

### Is there a reminder available for vendor bills pending approval? {#question_N2375470}

Yes. Go to the Home page > Reminders portlet > setup. Click Add Standard Reminders and add Bill to Approve.

### Without any workflow customization, can an email alert be sent to the designated approver? {#question_N2375492}

No, a custom workflow approval or a saved search is needed for this condition.

### Is there an Approve button when viewing a bill which is pending approval? {#question_N2375545}

No. You must do one of the following:

-   Edit the bill and set the approval status to Approved.
    
-   Use the Approve Bills page to set the approval status to Approved.
    
    See [Bulk Approving Vendor Bills With Standard Vendor Bill Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2374794.html).
    

### If the bill is rejected, can I create another bill from the same purchase order for approval? {#question_N2375616}

Yes. After a bill is rejected, the expense account, quantities and amount are zeroed and the purchase order status changes from Fully Billed to Pending Billing.

### Is there any General Ledger (GL) impact for a bill with a Pending Approval status? {#question_N2375637}

No. The GL impact reflects on a bill only when it is approved.

### Additional Information

-   [Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2376194.html)
-   [3 Way Match Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4096219721.html)
-   [Vendor Bill Approvals in the Employee Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157528106765.html)

### Related Topics

### Related Topics

-   [Approving Vendor Bills With Standard Vendor Bill Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2374450.html)
-   [Vendor Bill Approvals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2373552.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
