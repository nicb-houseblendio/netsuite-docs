---
id: "section_N1171932"
type: "section"
title: "Authorizing Individual Partner Commissions"
branch: "partners"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Partners > Partner Commissions & Royalties > Authorizing Partner Commission > Authorizing Individual Partner Commissions"
parent: "section_N1171542"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1171932.html"
anchors: ["procedure_N1171958"]
sha256: "8efacdcfe54dfb875c416afbad26636adaaa7140700e0babd021dd46f2e9e50d"
---

After NetSuite generates a commission amount from a sale that meets the commission criteria, it must be authorized. You must have the Partner Commission Transaction permission to authorize commission. The standard Sales Manager and Sales Administrator roles include this permission.

Authorization confirms the commission amount, creates a commission payable transaction, and may also give accounting approval to create a payment check.

#### To authorize individual commission transactions: {#procedure_N1171958}

1.  Go to _Transactions > Commissions > Individual Partner Commission_.
    
2.  In the **Partner** field, select the partner to which you want to pay the commission.
    
3.  In the **Account** field, select an account to which this commission payment should post.
    
    The balance for this account is shown in the **Balance** field.
    
4.  Select an account for this commission in the **Expense Account** field.
    
    You can set the default expense account for partner commission at _Setup > Sales > Sales Management > Commissions_.
    
5.  Accept or enter the date in the **Date** field.
    
6.  In the **Posting Period** field, select the period to which you want to post this commission transaction.
    
7.  In the **Date Eligible** field, enter a date to filter commission transactions by the date they became eligible.
    
    You can use this date filter to show only the transactions for the month you are authorizing.
    
    This date defaults to the most recent date for eligible transactions. For example, you have a commission eligibility period of 15 days and today's date is February 28. The Date Eligible field defaults to February 13. NetSuite lists only transactions that are eligible on the date you authorize commission.
    
    If you use the Multiple Currencies feature, the partner's currency appears in the **Currency** field.
    
    You can update the exchange rate for the partner's currency in the **Exchange Rate** field.
    
8.  In the **Memo** field, enter a memo for this transaction.
    
9.  Check the **Accounting Approval** box to approve payment of this commission.
    
    Note:
    
    You can check this box if you use the **Accounting Approval** preference and you are authorized to give accounting approval.
    
10.  Accept or enter the commission number in the **Commission #** field.
     
     If you use auto-generated numbering for commission transactions, you can change the commission number only if you allow override on commission transactions. For more information, see [Set Auto-Generated Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N252198.html).
     
11.  If you want to associate this commission transaction with a department, location, or class, select it in the corresponding field.
     
12.  Choose the amounts to include on the commission transaction:
     
     -   Include a commission on the **By Transaction** subtab by checking the box next to the commission.
         
     -   Include a commission on the **By Period** subtab by checking the box next to the commission.
         
         The following columns appear on the **By Transactions** and **By Period** subtabs:
         
         -   **Date Eligible** - The date the commission is eligible based on the terms of the schedule plus the offset preference
             
             This column appears only on the **By Transaction** subtab.
             
             For example, an order closed on 6/1/2019 has an eligibility schedule based on billings and the order is invoiced on 6/15/2019. The eligible date is 6/15/2019. If the offset is 5 days, the eligible date is 6/20/2019.
             
         -   **Calculated Commission** - The amount calculated by the schedule, which is the total payable amount
             
         -   **Previously Authorized** - The amount that was previously authorized
             
             In view mode, this is the total amount authorized including this transaction.
             
         -   **Eligible Amount** - The total amount that is eligible after the triggering event occurs (billing or collection)
             
             Note:
             
             This amount may differ from the calculated commissions column. For example, if a schedule is based on collections and you received half the payment, the eligible amount is half the calculated amount.
             
         -   **Amount** - The amount authorized by this transaction
             
     -   Enter a commission amount manually by clicking the **Other Commissions** subtab and filling in a **Memo** and **Amount** for the commission. Click **Add**.
         
         The **Exchange Rate** column displays the currency exchange rate on the date you authorize this commission. The **Foreign Currency Amount** column displays the related commission amount.
         
13.  Click **Save**.
     

The Processed Partner Commissions page displays the status of the commission authorization process while the process is running. Displayed information includes the name of the partner receiving the commission and the status of the commission payment. It also includes any transaction number, amount of the commission payment, and any processing error.

Note:

You can't authorize commissions for partners whose commissions are currently being authorized.

If you use the Require Accounting Approval of Partner Commissions preference, authorized commission must be approved by your accounting department. Go to _Setup > Sales > Sales Management > Commissions_ to set the preference.

If you do not require accounting approval, you can pay authorized commission at _Transactions > Payables > Pay Bills_.

### Related Topics

-   [Setting Up a Partner for Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1169829.html)
-   [Creating a Partner Commission Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1171112.html)
-   [Viewing the Status of Authorized Partner Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3801365103.html)
-   [Approving Partner Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1173679.html)
-   [Authorized Partner Commission Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1175260.html)
-   [Authorized Partner Commission Summary Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1175063.html)
-   [Landed Cost and Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2420792.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
