---
id: "section_N1171714"
type: "section"
title: "Authorizing Partner Commission in Bulk"
branch: "partners"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Partners > Partner Commissions & Royalties > Authorizing Partner Commission > Authorizing Partner Commission in Bulk"
parent: "section_N1171542"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1171714.html"
anchors: ["procedure_N1171734"]
sha256: "31683a183db92616b0bf213a7750db4de584b57ec5533ee61728f7efe6b484dc"
---

After NetSuite generates a commission amount from a sale that meets the commission criteria, it needs to be authorized. You must have the Partner Commission Transaction permission to authorize commission. The standard Sales Manager and Sales Administrator roles include this permission.

Authorization confirms the commission amount, creates a commission payable transaction, and may also give accounting approval to create a payment check.

Bulk partner commission transactions source department, class, and location from partner records.

#### To authorize bulk commission transactions: {#procedure_N1171734}

1.  Go to _Transactions > Commissions > Authorize Partner Commissions_.
    
    The Authorize Partner Commissions page displays a list of commission transactions pending authorization.
    
2.  Select the date on which you want to authorize the commission transactions.
    
3.  Select the period to which these commission transactions should post.
    
4.  Check the **Accounting Approval** box to give accounting approval for these commission transactions.
    
    Commission transactions with accounting approval can be paid through checks.
    
5.  In the **Account** field, select the account to which you want these commission transactions to post.
    
    The balance for this account is shown in the **Balance** field.
    
6.  Select the expense account used by these commission transactions.
    
7.  In the **Date Eligible** field, enter a date to filter commission transactions by the date they became eligible.
    
    You can use this date filter to show only the transactions for the month you are authorizing.
    
    This date defaults to the most recent date for eligible transactions. For example, if you have a commission eligibility period of 15 days and today's date is February 28, the **Date Eligible** field defaults to February 13. NetSuite lists only transactions that are eligible on the date you authorize commission.
    
8.  In the **Select** column, check the box next to one or more commission amounts to authorize, or click **Mark All**.
    
9.  Click **Authorize**.
    

The Processed Partner Commissions page displays the status of the commission authorization process while the process is running. Information that displays includes the name of the partner receiving the commission and the status of the commission payment. It also includes any transaction number, amount of the commission payment, and any processing error.

Note:

You can't authorize commissions for partners whose commissions are currently being authorized.

If you use the Require Accounting Approval of Partner Commissions preference, authorized commission must be approved by your accounting department. Go to _Setup > Sales > Sales Management > Commissions_ to set the preference.

If you do not require accounting approval, you can pay authorized commission at _Transactions > Payables > Pay Bills_.

### Related Topics

-   [Setting Up a Partner for Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1169829.html)
-   [Creating a Partner Commission Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1171112.html)
-   [Approving Partner Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1173679.html)
-   [Viewing the Status of Authorized Partner Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3801365103.html)
-   [Authorized Partner Commission Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1175260.html)
-   [Authorized Partner Commission Summary Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1175063.html)
-   [Landed Cost and Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2420792.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
