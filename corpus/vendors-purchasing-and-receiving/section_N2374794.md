---
id: "section_N2374794"
type: "section"
title: "Bulk Approving Vendor Bills With Standard Vendor Bill Approval"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Bills > Vendor Bill Approvals > Bulk Approving Vendor Bills With Standard Vendor Bill Approval"
parent: "section_N2373552"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2374794.html"
anchors: ["procedure_N2374819", "bridgehead_N2374909"]
sha256: "95b536dd8035099892c5f5d51f366b2be405169a91ac22d847e4da753a182c8d"
---

After you enter vendor bills, any bill with a status of Pending Approval or Rejected must be set to Canceled or Approved. To save time, you can run a bulk process to approve many vendor bills at one time.

The Approve Bills page lists all bills that require approval.

#### To bulk process vendor bill approvals: {#procedure_N2374819}

1.  Go to _Transactions > Payables > Approve Bills_.
    
2.  Select a vendor to filter the list of bills.
    
3.  Select a date range to filter the list of bills that show. The date range you select is reflected in the **From** and **To** fields.
    
    If you enter a different range in the **From** and **To** fields, the **Date** field automatically shows Custom.
    
4.  Check the box in the **Approve** column next to a bill to approve it.
    
    Click **Mark All** to select all bills for approval.
    
5.  Optionally click the **Select Order Number** field to enter or scan an order number.
    
6.  As you mark bills to be approved, the total is displayed in the **Amount** field in the header.
    
7.  Click **Submit**.
    

Now, the bills you marked have a status of Approved and can be processed for payment.

## Bulk Approval Queue Errors {#bridgehead_N2374909}

When you are bulk approving vendor bills, it is possible for an error to occur during processing. For example, you may submit ten bills in the approval queue. The first four are processed and approved without difficulty, but the fifth bill encounters an error. In such a case, the processing immediately stops and the error is reported.

The first four bills have an Approved status. However, the fifth and subsequent bills still require approval. You should approve the fifth bill individually, and then resubmit the remaining bills (six through ten) that remain in the approval queue.

### Additional Information

-   [Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2376194.html)
-   [3 Way Match Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4096219721.html)
-   [Vendor Bill Approvals in the Employee Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157528106765.html)

### Related Topics

### Related Topics

-   [Setting the Default Vendor Approval Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2374176.html)
-   [Approving Vendor Bills With Standard Vendor Bill Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2374450.html)
-   [Standard Vendor Bill Approval FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2375312.html)
-   [Vendor Bill Approvals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2373552.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
