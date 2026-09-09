---
id: "section_N1288824"
type: "section"
title: "Applying a Payment on the Customer Payment Page"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Customer Payments > Applying a Payment on the Customer Payment Page"
parent: "section_N1285644"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1288824.html"
anchors: ["bridgehead_4586576967", "bridgehead_1515768819", "bridgehead_4594345165", "bridgehead_4586857902", "bridgehead_4586865850", "bridgehead_4586866149", "bridgehead_4586866903", "bridgehead_1530146538"]
sha256: "f7b8f89faef2f3f3b3dbf419afdf0810ac3df80479487605a39ba663f597ddd9"
---

Use the Customer Payment page to record a customer payment. On this page, you can perform the following tasks:

-   [Recording a Customer Payment](#bridgehead_4586576967)
    
-   [Adding Additional Information to a Customer Payment](#bridgehead_4594345165)
    
-   [Adding Payment Information to a Customer Payment](#bridgehead_4586857902)
    
-   [Applying Credits and Deposits to a Customer Payment](#bridgehead_4586865850)
    
-   [Adding Relationships to a Customer Payment](#bridgehead_4586866149)
    
-   [Adding Communication Information to a Customer Payment](#bridgehead_4586866903)
    
-   [Adding EFT Information to a Customer Payment](#bridgehead_1530146538)
    

![Example of a NetSuite Payment record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/SA-PaymentsForm.png)

## Recording a Customer Payment {#bridgehead_4586576967}

The minimum information you need to record a customer payment is:

-   Customer
    
-   Payment Amount
    
-   Accounts receivable account.
    
    If you have only one Accounts Receivable account listed in the Chart of Accounts, NetSuite defaults this account as the posting account for customer payments.
    

#### To record a customer payment:

1.  Go to _Customers > Accounts Receivable > Accept Customer Payments_.
    
2.  In the **Customer** field, select the customer or project you want to accept payment from.
    
3.  In the **A/R Account** field, select a posting account for this transaction.
    
    Only invoices charged to this account show in the list.
    
    Note:
    
    If you do not see this field, this means you have only one Accounts Receivable account in your chart of accounts.
    
4.  If you use the Classification feature, select a department, class, or location to associate this transaction with a classification.
    
    Note:
    
    If you use NetSuite OneWorld and the selected customer is shared with multiple subsidiaries, you can choose any subsidiary assigned to the selected customer. For information about sharing customer records with multiple subsidiaries, see [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
    
5.  On the **Apply** subtab, enter the amount received in one of the following ways:
    
    -   Enter the received amount in the **Payment Amount** field, and then check the **Auto Apply** box.
        
    -   Leave the **Payment Amount** field empty and select invoices to which you want to apply the payment.
        
    -   Enter the received amount in the **Payment Amount** field and check the boxes next to each invoice.
        
        You can check only those invoices that can be covered by the payment amount you entered.
        
    -   Enter the received amount in the **Payment Amount** and clear all boxes next to invoices if you do not want to apply this payment to any open invoices.
        
6.  To enter a discount for an invoice manually, enter the discount amount in the **Discount Taken** field for this invoice.
    
7.  Click **Save**
    

Important:

When processing transactions, you must submit one page at a time. If you do not submit each page individually, information is not saved and can be lost when you switch between pages. To process multiple pages of information, always submit each page individually.

If you make payment for a customer for an amount that is larger than the amount owed, a customer deposit is created for the remaining payment amount.

NetSuite remembers your preference for using the Auto Apply box on the Apply subtab of customer payments. The next time you enter a customer payment, the Auto Apply box is checked or cleared by default based on the last payment you entered.

## Customer Payments with a Payment Amount of Zero after Applying a Discount {#bridgehead_1515768819}

When you apply credit and a discount that result in a **Payment Amount** of zero, a **Customer Payment** is still created.

The **Customer Payment** is needed to track the discount, which has an impact on the general ledger.

## Adding Additional Information to a Customer Payment {#bridgehead_4594345165}

The customer payment Primary Information section contains fields that let you specify additional information, such as the accounts where funds are posted and currency.

The following table lists additional information you can specify for the customer payment.

| Account | If you are entering a payment that has already been deposited, select Account, and then select the the bank account. |
| --- | --- |
| Udep. Funds | If you receive payment by cash or check and your bank account is not credited until you actually make the deposit, select **Undep. Funds**. You can later go to _Transactions > Bank > Make Deposits_ |
| Date | The current date shows in the Date field. You can select or enter another date. What you enter here determines the date range in which this transaction appears on the Accounts Receivable register. |
| Currency | If you use the Multiple Currencies feature, select the currency of the invoices to which you want to apply payment. Selecting a currency in this field filters the list of invoices, credit memos, and deposits available under the Apply subtab. If you create a payment from an invoice and then select a different currency on this page, the original invoice is filtered from the list on the Invoices subtab. For more information, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html). |

## Adding Payment Information to a Customer Payment {#bridgehead_4586857902}

To add a payment method and other payment information on the Customer Payment page, follow the instructions in [Entering Payment Information on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586835857.html).

## Applying Credits and Deposits to a Customer Payment {#bridgehead_4586865850}

You can apply open credit memos, unapplied payments, and prepayments to invoices on the customer payment page.

Note:

The unapplied part of customer deposit created from sales order can be used as a credit on a customer payment only when sales order status is billed, canceled, or closed.

#### To apply credits and deposits to a customer payment:

1.  On the Customer Payment page at _Customers > Accounts Receivable > Accept Customer Payments_.
    
2.  On the **Apply** subtab:
    
    1.  Click the **Credits** subtab to apply open credit memos:
        
        -   Check the box in the **Apply** column next to each credit memo you want to apply.
            
        -   Clear the box in the **Apply** column next to each credit memo you are not applying.
            
        -   Click **Mark All** to apply all existing credits.
            
    2.  Click the **Deposits** subtab to apply a customer prepayment to an invoice:
        
        -   Check the box in the **Apply** column next to each customer deposit you want to apply.
            
        -   Clear the box in the **Apply** column next to each customer deposit you are not applying.
            
        -   Click **Mark All** to apply all existing customer deposits.
            
3.  Click **Save**.
    

## Adding Relationships to a Customer Payment {#bridgehead_4586866149}

You can associate the customer's contact information with a customer payment. Click the Relationships subtab to enter the contact information. For more information, see [Entering Relationships on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586861907.html)

## Adding Communication Information to a Customer Payment {#bridgehead_4586866903}

Use the Communication subtab to create and send messages to your customers from the Customer Payment page. For more information, See [Entering Communication Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586862223.html).

## Adding EFT Information to a Customer Payment {#bridgehead_1530146538}

If you are using Electronic Bank Payments for customer direct debit payment transactions, you can assign which entity bank account the payment will be debited from.

Note:

When processing customer payments through electronic bank payments, make sure the For Electronic Bank Payment (Direct Debit) is checked under Payment Method subtab.

#### To apply your preferred entity bank to a customer payment:

1.  Go to the Customer Payment page at _Customers > Accounts Receivable > Accept Customer Payments_.
    
2.  Click the EFT subtab to select the preferred entity bank account to be used with this transaction.
    
    -   **Preferred Entity Bank** - By default, the primary entity bank account of the customer will be selected in this field. You can select from the dropdown list if you want to use any of the secondary bank accounts available in the Customer record. For more information, see the country-specific topics about Setting Up Bank Records for Customers for Electronic Bank Payment.
        
    -   **Entity Bank Details** - This field displays the entity bank details based on the preferred entity bank account selected for this payment.
        
3.  Click **Save**.
    

### Related Topics:

-   [Accepting Customer Payments Workflow Chart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1285644.html#section_N1288273)
-   [Applying a Payment on an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1289458.html)
-   [Correcting Payments to Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1292877.html)
-   [Entering Payment Information on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586835857.html)
-   [Removing Credits from Deleted Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1292961.html)
-   [Reversing or Deleting Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4744566376.html)
-   [Approving Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4373987935.html)
-   [Managing Undeposited Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1294497.html)
-   [Consolidated Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1288474.html)
-   [Payment Receipts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1293235.html)
-   [Creating a Payment Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1292421.html)
-   [Handling Returned/NSF Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1295030.html)
-   [Allowing Customers to Pay Online](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1293669.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
