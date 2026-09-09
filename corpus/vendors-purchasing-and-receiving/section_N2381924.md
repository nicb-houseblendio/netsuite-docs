---
id: "section_N2381924"
type: "section"
title: "Paying Bills to a Single Vendor"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Payments > Paying Bills to a Single Vendor"
parent: "chapter_N2381615"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2381924.html"
anchors: ["bridgehead_1496250966", "procedure_N2381948", "bridgehead_1496250991", "procedure_N2383500"]
sha256: "6acfdaab20a55e352448a11c939820bea04ec54069411e6bcf987d09d9c1ba45"
---

Use the Pay Single Vendor transaction to pay for outstanding payables to one vendor. You can also select an employee in the Payee field to pay employee expenses.

You can"t make payments to inactive vendors. For more information, see [Inactivating Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4443201053.html).

Note:

All system-generated currency revaluation including rounding revaluation posts to the current open period. This enables you to move the revaluation to any period you require.

Use these links for more information about two methods to pay these bills:

-   [Make a bill payment to a single vendor](#bridgehead_1496250966)
    
-   [Pay a single vendor from a bill](#bridgehead_1496250991)
    

## Make a bill payment to a single vendor {#bridgehead_1496250966}

#### To make a bill payment to a single vendor: {#procedure_N2381948}

1.  Go to _Transactions > Payables > Pay Single Vendor_.
    
2.  Check the **To ACH** box.
    
3.  Complete the form as described in the following sections.
    
4.  Click **Save**.
    

After the bill is paid, you can view bill payments by going to _Transactions > Payables > Enter Bills > List_. The Credits Applied subtab on payments shows any credits that were applied.

If you are offsetting bills or refunds with credits and no balance is due, the transactions are updated and no payment checks are created.

#### Primary Information

1.  In the **A/P Account** field, select an accounts payable account for this transaction.
    
2.  From the **Custom Form** field, select a form to use for this transaction.
    
    Note:
    
    This field appears only if you have a custom bill payment form available. NetSuite sets the standard bill payment form otherwise.
    
3.  In the **Payee** field, select the payee you want to pay.
    
    -   Select a vendor to pay a vendor bill.
        
        If you use NetSuite OneWorld and this vendor is shared with multiple secondary subsidiaries, the **Subsidiary** field defaults to the vendor's primary subsidiary. You can, however, change it to any secondary subsidiary assigned to this vendor. For more information about globally shared vendor records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).
        
        If the vendor record you select is not shared with multiple subsidiaries, the **Subsidiary** field defaults to the vendor's assigned subsidiary.
        
    -   Select an employee to pay an expense report.
        
    
    Outstanding payables for this payee appear in the list.
    
    If you use multiple currencies, the currency for this vendor appears in the **Currency** field.
    
4.  In the **Account** field, select an account for this transaction
    
5.  The **Balance** field displays the balance in the selected account.
    
6.  If you use the Multiple Currencies for vendors feature, select the currency of the bills you want to pay. This filters the list of bills to show only the bills in this currency. For more information, see [Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395463.html) and [Vendors and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1400742.html).
    
7.  The exchange rate for this currency is shown in the **Exchange Rate** field. You can enter an exchange rate for this currency.
    
8.  The current date shows, but you can select or enter another date.
    
9.  Select the period you want this payment to post to.
    
    If you use approval routing, the posting period is set upon approval. For details, see [Posting Period for Transactions Subject to Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2394992.html#subsect_156806140378).
    
10.  On the **Payee Address** subtab, the address information from the payee records appears. If the **Auto Fill** preference is enabled, the address information from the latest transaction for the payee appears. If you have not pay any invoices to the contact or if the **Auto Fill** preference is disabled, the **Default Billing** address information appears.
     
     Note:
     
     The **Auto Fill** preference takes precedence over the **Default Billing** address.
     
     To check or clear the **Default Billing** box, go to _Home > Set Preferences_ List > Relationships > Customers. Click **Edit** next to a customer. This box is on the **Address** subtab, next to an address.
     
11.  Check the appropriate box:
     
     -   **To Be Printed** - adds a check to the print queue
         
     -   **Voucher** - adds a voucher for this check to the print queue
         
12.  The **Check #** field shows the next check number or shows To Bill Pay.
     

#### Classification

1.  Select a **Department**, **Class**, and **Location**, if you track them.
    
2.  Check the **For Electronic Bank Payment** box if you want to process the payment transaction through Electronic Payments. When this box is checked, the Check # field and other payment options are automatically cleared.
    
3.  The **Vendor Bank Fees** field value is dependent on the payee selected. This field identifies if the vendor or company will pay the bank transfer fee. For more information, see help topic [Japan Zengin Bank Fee Calculation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530060823.html).
    

#### Apply Subtab

1.  On the **Apply** subtab, check the **Apply** box next to bills you want to pay.
    
    As you apply bills, the total payment amount is shown in the **Amount** field.
    
    Important:
    
    The **Amount Due** field is dynamically calculated.
    
    Amount Due = Vendor Bill amount - (Other credit applied to the bill and other payment applied on the bill).
    
2.  Check the **Apply** box next to credits you want to apply.
    

#### Relationships

1.  On the **Relationships** subtab, the primary contact for the customer is selected automatically. To edit information for this contact, click the contact name.
    
    You can also add contacts to this order by entering the contact information and clicking **Add**.
    

#### Communication

1.  Click the **Communication** subtab to associate activities, notes or files with this transaction.
    
    -   Use the **Events**, **Tasks**, and **Phone Calls** subtabs to attach activities to this transaction. For more information, see [Attaching Events, Tasks, and Calls to Records and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1084924.html).
        
    -   On the **Files** subtab, you can select and attach files from the File Cabinet related to this transaction. Select **New** to upload a new file to File Cabinet.
        
    -   On the **User Notes** subtab, you can enter a title and note for any comments you want to add to this transaction. Click **Add** after each note.
        

#### EFT Subtab

1.  Click the **EFT** subtab to select the preferred bank account to pay outstanding payments to a single vendor, employee, or partner for electronic bank payment.
    
    -   **Preferred Entity Bank** - By default, the primary entity bank account of the payee will be selected in this field. You can select from the dropdown list if you want to use any of the secondary bank accounts available in the payee record. For more information, see the country-specific topics about Setting Up Bank Records for Vendors, Employees, and Partners for Electronic Bank Payment.
        
    -   **Entity Bank Details** - This field displays the entity bank details based on the preferred entity bank account selected for this payment.
        

You can also pay a vendor directly from an existing bill.

## Pay a single vendor from a bill {#bridgehead_1496250991}

#### To pay a single vendor from a bill: {#procedure_N2383500}

1.  Go to _Transactions > Payables > Enter Bills_.
    
2.  Click **View** next to the bill you want to pay.
    
3.  On the bill, click the **Make Payment** button.
    
4.  Check the **To ACH** box.
    
5.  Verify that the payment information showing on the bill is correct.
    
6.  Check the **Apply** box next to credits you want to apply.
    
7.  Check the appropriate box:
    
    -   **To Be Printed** - adds a check to the print queue
        
    -   **Voucher** - adds a voucher for this check to the print queue
        
8.  Click **Save**.
    

### Related Topics

-   [Vendor Payments Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2381751.html)
-   [Default Vendor Payment Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161037364692.html)
-   [Paying Bills to Multiple Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2383803.html)
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
