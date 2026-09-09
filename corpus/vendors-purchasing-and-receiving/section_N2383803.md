---
id: "section_N2383803"
type: "section"
title: "Paying Bills to Multiple Vendors"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Payments > Paying Bills to Multiple Vendors"
parent: "chapter_N2381615"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2383803.html"
anchors: ["procedure_N2383828"]
sha256: "d04b556de0ddf4363ffd62930e40331e4336d79b68890743d39afd91a06ac037"
---

Use NetSuite to process payments to several vendors at one time.

Note:

You can"t make payments to inactive vendors. For more information, see [Inactivating Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4443201053.html).

All system-generated currency revaluation including rounding revaluation posts to the current open period. This enables you to move the revaluation to any period you require.

#### To pay multiple vendors: {#procedure_N2383828}

1.  Go to _Transactions > Payables > Pay Bills_.
    
2.  In the **A/P Account** field, select an accounts payable account to associate with this payment.
    
3.  In the **Account** field, select the bank account you are using to pay these bills. When you select an account, the current balance of the account appears in the **Balance** field.
    
4.  The **Balance** field shows the balance in the account you selected.
    
5.  The current date autofills the **Date** field.
    
6.  Select the period you want this payment to post to.
    
7.  Select a department, class and location, if you track them.
    
    If a custom segment is applied on the vendor payment record, the custom segment field is displayed in the Classification section. Select the custom segment to apply to all vendor payments.
    
8.  Enter a date in the **Start Date** field to limit the transactions in the list.
    
    The **Start Date** field is blank by default and all open payable transactions appear in the list.
    
    Entering a start date and end date in their respective fields filters your list of payable transactions by due date.
    
    Note:
    
    If you enter a start date and an end date, payable transactions without a due date entered won't appear on the list.
    
9.  If you want to print your bill payments, check the **To Be Printed** box.
    
10.  In the **Use Bill-To Address From Vendor** field, do the following:
     
     -   Check this box to use the vendor's default billing address on bill payments generated regardless of the billing address shown on the bill or credit.
         
         If a vendor has no default billing address, the **Address** field on bill payment is blank.
         
     -   Clear this box to use the billing address shown on the bill or credit for bill payments that are generated.
         
     
     Journal entries always use the current default billing address of the vendor.
     
11.  Click the Select Item to scan in transaction bar codes.
     
12.  Check the box in the **Pay** column next to the bills you want to pay and the credits you want use to offset the bills.
     
     Note:
     
     There must be at least ten transactions for NetSuite to split the transactions into multiple workqueue records.
     
     This list shows your outstanding bills, and any credits or refunds you have received from vendors. This list also includes expenses due to be paid to employees.
     
     Note:
     
     If you use the Multiple Currencies feature, the bills showing in the list depend on currency settings.
     
     If you use NetSuite OneWorld, only bills associated with the subsidiary where the account can be used shows in the list. If the account currency is the same as the subsidiary's currency, all bills associated with the subsidiary show in the list, regardless of the currency. If the account currency is different from the subsidiary's currency, only bills associated with the subsidiary and with the account currency show in the list.
     
     If you do not use NetSuite OneWorld, note the following. If the account currency is the same as the base currency, all bills show in the list, regardless of currency. If the account currency is different from the base currency, only bills that use the account currency show in the list.
     
     As you check bills and credits, the total amount of the payment appears in the **Amount** field at the top of the page.
     
     This amount is shown in your base currency. If you use the Multiple Currencies feature and have bills in other currencies selected, those currency amounts are converted into your base currency. For more information, see [Vendors and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1400742.html).
     
     For accounts that use the Electronic Bank Payments SuiteApp, bank fee is calculated as soon as the payment records are processed. The **Bank Fee** field is calculated for each payment when:
     
     -   The bank account selected is associated with a company bank detail account that uses a Zengin template.
         
     -   The **EFT Bill Payment** box is checked on the vendor record.
         
     
     For more information about bank fee calculation, see [Japan Zengin Bank Fee Calculation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530060823.html).
     
     You can click the date next to a bill or credit to open it.
     
     #### To open the vendor record:
     
     1.  Click the vendor **Name**.
         
     2.  Click **Mark All** to select all bills that show on the page you are viewing.
         
         If the list of bills extends beyond one page, you must view the next page of results to select those bills.
         
     3.  On additional pages, you can select individual bills or click **Mark All** to select all the bills that are showing.
         
     4.  After you have marked the bills to pay in the list, click **Save** to submit them for payment .
         
     
13.  Click **Save** to process the bill payments.
     

If you are offsetting bills with credits or returns and no balance is due, the transactions are updated and no payment checks are created.

### Related Topics

-   [Vendor Payments Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2381751.html)
-   [Default Vendor Payment Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161037364692.html)
-   [Paying Bills to a Single Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2381924.html)
-   [Checking the Status of a Bill Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4401801571.html)
-   [Editing a Bill Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2384435.html)
-   [Correcting Bill Payment Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2385178.html)
-   [Printing Bill Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2384738.html)
-   [Printing Bill Payment Vouchers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2384154.html)
-   [Vendor Payment Installments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1550603013.html)
-   [In-Transit Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1535398724.html)
-   [Custom Workflow-Based Approvals for Vendor Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554290907.html)
-   [Vendor Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2381615.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
