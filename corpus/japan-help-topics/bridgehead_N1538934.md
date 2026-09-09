---
id: "bridgehead_N1538934"
type: "bridgehead"
title: "Applying a Customer Payment to an Invoice Summary"
branch: "japan-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Japan Help Topics > Japanese Invoicing > Japanese Invoice Summary > Applying a Customer Payment to an Invoice Summary"
parent: "section_N1536907"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1538934.html"
anchors: ["procedure_N1538954", "procedure_N1539046"]
sha256: "597d38121ecd765d5bc1397d6dadbed90f6e8245cbafb505760fc010fb1db7cc"
---

When accepting a customer payment, select the invoice summary that the payment should be applied to. You can also view the invoice summary numbers associated with the invoices on the payment sublist, where the Invoice Summary Number column isn't displayed by default. You should customize the payment sublist to display the Invoice Summary Number column. Set this up one time only. When the column is set up, it's always displayed when you open a customer payment page.

#### To customize the payment sublist to show the Invoice Summary Number column: {#procedure_N1538954}

1.  Go to Transactions > Customers > Accept Customer Payments.
    
2.  On the **Apply** subtab, click **Customize**.
    
3.  On the Customize Sublist page, on the **Additional Columns** subtab, check the **Invoice Summary Number** box.
    
    The **Invoice Summary Number** column is now displayed every time you open a customer payment page.
    

#### To apply a customer payment to an invoice summary: {#procedure_N1539046}

1.  Go to Transactions > Customers > Accept Customer Payments > List.
    
2.  Click the Edit link of the customer that you want to accept payments from, or click **New** to create a new Payment record.
    
3.  Enter values in the required fields.
    
4.  On the **Apply** subtab, in the **Apply to Invoice Summary** field, select the invoice summary number that this payment should be applied to.
    
    Only open invoice summaries are available in the dropdown list.
    
    ![Accept Payment Terms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/CountrySpecificFeatures/Japan_AcceptCustomerPayment_inRedwood.png)
    
    Note:
    
    NetSuite automatically checks the **Apply** box for invoices that are included in the selected invoice summary number, while disabling Auto Apply. The invoice summary number of those invoices are displayed in the **Invoice Summary Transaction** column.
    
5.  If there are individual invoices that you want to apply this payment to, check the **Apply** box for those invoices.
    
    Note:
    
    The marked invoices won't be included in the invoice summary . NetSuite treats them as individual invoices to which the amount on the payment record is also applied.
    
6.  Click **Save**.
    

In case you need to reconcile any customer payments, you can open the Customer Payment record and view the invoice summary numbers associated with the invoices.

When the invoice summary is generated, the total of customer payments and deposits are included. Total advance payments from customers, recorded as Customer Deposits, are indicated under Payments Received This Period in the invoice summary, and in a column with the same label in its PDF file.

Note:

In addition to applying customer payments to invoice summaries, you must consider these cases:

-   AR Debit/Credit Adjustment transactions that were created from invoice summaries with Apply Invoice Summary Tax Adjustment enabled and an AR Debit/Credit Adjustment Item selected, can be included in the Customer Payment record. The Apply box of an AR Debit/Credit Adjustment transaction is automatically checked if the Apply box of its source invoice summary is checked. However, AR Debit/Credit Adjustment transactions that were created manually, aren't automatically included in the payment record.
    
-   Generated invoice summaries with any of its transactions deleted, shouldn't be included in the Customer Payment record; otherwise, this will result in invalid data and an error will be encountered.
    

### Related Topics

-   [Japanese Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1536907.html)
-   [Setting the Invoice Summary Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1547537829.html)
-   [Specifying Customers Who Use Invoice Summaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1537000.html)
-   [Specifying Transactions for Inclusion in an Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1537181.html)
-   [Including Payment Adjustments in the Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159954224986.html)
-   [Adding Field Values to the Invoice Summary Output](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1547538342.html)
-   [Specifying a Folder to Save Invoice Summaries In](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159954596474.html)
-   [Generating a Japanese Invoice Summary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1539302.html)
-   [Regenerating an Invoice Summary for a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4355754839.html)
-   [Viewing Invoice Summary Generation Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159953645373.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
