---
id: "section_N1234186"
type: "section"
title: "Creating Terms of Payment"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Billing > Creating Terms of Payment"
parent: "chapter_4419712298"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234186.html"
anchors: ["procedure_N1234206"]
sha256: "d1eda06dfe450919ad8599e246c8b3e2399b154f26077bcedae695564036e348"
---

Terms are used to specify when payment is due on customer invoices and vendor bills. Define the specific requirements of a term of payment by creating a term record. You can create different payment terms for different customers or vendors.

#### To create a standard term record: {#procedure_N1234206}

1.  Go to _Billing > Setup > Payment Terms > New_.
    
2.  On the Add to Accounting List page, select **Term**.
    
3.  On the Term page, select **Standard**.
    
    Note:
    
    Standard is selected by default, as opposed to Date Driven.
    
4.  Enter a name for the term in the **Terms** field.
    
    For example, you can name a term **Net 30**.
    
5.  In the **Days Till Net Due** field, enter the number of days until the net amount of the invoice or bill becomes due.
    
6.  In the **% Discount** field, enter the percentage discount if the invoice or bill is paid early.
    
7.  In the **Days Till Discount Expires** field, enter the number of days the early payment discount is available.
    
    For example, if the early payment discount is available for 15 days after the bill is issued, enter **15** in this field.
    
8.  Click **Save**.
    

#### To create a date driven term record

1.  Go to _Billing > Setup > Payment Terms > New_.
    
2.  On the Term page, select **Date Driven**. Date driven terms are used when payment is due on a particular calendar date; for example, the 15th of the month.
    
3.  Enter a name for the term in the **Terms** field.
    
4.  In the **Day of Month Net Due** field, enter the day of the month when the net amount of the invoice is due.
    
    If you enter a date that doesn't exist in the month the transaction is due, the last day of the month becomes the due date.
    
5.  In the **Due Next Month If Within Days** field, enter the number of days before the due date during which issued invoices will be carried forward to the next month.
    
    Use this field to make sure customers are always given a minimum number of days to pay after they're invoiced.
    
    For example, if invoices are due on the 30th of each month and you enter **5** in this field, then invoices issued between the 25th and 30th are due for payment by the 30th of the following month.
    
6.  In the **% Discount** field, enter the percentage discount if the invoice is paid early.
    
7.  If you offer a discount for early payment, enter the last day of the month the early payment discount is available in the **Day Discount Expires** field.
    
    For example, if the early payment discount is available through the 20th of each month, enter **20** in this field.
    
8.  Check the **Preferred** box if you want to use this term for customers by default.
    
9.  Click **Save**.
    

Now this term can be used on customer records, vendor bills and other transactions.

You can create several term records to apply the appropriate terms to individual customers, vendor bills and other transactions. Standard terms include the following:

-   1% 10 Net 30
    
-   2% 10 Net 30
    
-   Due on receipt
    
-   Net 15
    
-   Net 30
    
-   Net 60
    

You can apply the terms to invoices by choosing a term on individual invoices or by setting default terms on customer and vendor records. For more information, read [Using Terms of Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234578.html).

### Related Topics

-   [Deciding Between Invoices and Cash Sales](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233061.html)
-   [Statement Charges](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233128.html)
-   [Adding Billing Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588267772.html)
-   [Using Billing Classes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233375.html)
-   [Using Consolidated Billing for Projects and for Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1233909.html)
-   [Creating Terms of Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234186.html)
-   [Using Terms of Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234578.html)
-   [Remittance Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234795.html)
-   [Printing Remittance Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234980.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
