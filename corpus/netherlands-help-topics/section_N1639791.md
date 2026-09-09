---
id: "section_N1639791"
type: "section"
title: "Setting Up Bank Records of Customers in the Netherlands"
branch: "netherlands-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Netherlands Help Topics > Netherlands-Specific SuiteApp > Netherlands Localization > Netherlands Payment Formats > Setting Up Bank Records of Customers in the Netherlands"
parent: "section_N1636146"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1639791.html"
anchors: ["procedure_N1639803"]
sha256: "29b2db10dcaf8d805f618fc49650c9c998d7186afd29dc6e00415ac7e10bcfc2"
---

Set up the bank account details of each customer from whom you'll receive direct debit payments. You also need to set up the bank account details of each customer to whom you'll send customer refunds. You can set up several bank accounts for each customer.

#### To set up bank details of a customer for direct debit transactions:

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click **Edit** next to the name of the customer from whom you want to receive direct debit payments.
    
3.  On the **Bank Payment Details (Debit)** subtab, check the **Direct Debit** box.
    
4.  Click **Save**.
    
5.  On the **Bank Payment Details (Debit)** subtab, click **New Bank Details**.
    
6.  In the Payment File Format field, select SEPA Direct Debit (ABN AMRO).
    
7.  Fill-in the required fields depending on the payment format you selected.
    
    For more information, see [Netherlands Entity Bank Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159921152297.html).
    
8.  Click **Save**.
    

#### To set up bank details of a customer for refund transactions: {#procedure_N1639803}

1.  Go to _Lists > Relationships > Customers_.
    
    For information about creating a customer record, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).
    
2.  Click **Edit** next to the name of the customer to whom you want to send refund payments.
    
3.  On the **Bank Payment Details (Credit)** subtab, check the **EFT Customer Refund Payment** box.
    
4.  Click **Save**.
    
5.  Click **New Bank Details**.
    
6.  In the Payment File Format field, select any of the following: Equens-ClieOp, Equens-ClieOp (ING Bank), SEPA Credit Transfer (HSBC), or SEPA Credit Transfer (Netherlands).
    
    Important:
    
    Select **Equens-ClieOp (ING Bank)** if you're setting up the customer's account in a bank that belongs to the ING Group. Select **Equens-ClieOp** to set up the customer's account in other Dutch banks. ING banks supports variant B of the ClieOp format while the other Dutch banks supports variant C.
    
7.  Fill-in the required fields depending on the payment format you selected.
    
    For more information, see [Netherlands Entity Bank Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159921152297.html).
    
8.  Click **Save**.
    

You can also set up bank records of vendors by importing bank details in CSV format into NetSuite using the CSV Import Assistant. For more information, see [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html). The required fields on the employee record are also required in the CSV import.

### Related Topics

-   [Setting Up Company Bank Records in the Netherlands](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1636511.html)
-   [Setting Up Bank Records of Vendors in the Netherlands](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1638884.html)
-   [Setting Up Bank Records of Employees in the Netherlands](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1639339.html)
-   [Setting Up Bank Records of Partners in the Netherlands](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851230281.html)
-   [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html)
-   [Netherlands Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1636146.html)
-   [Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1585433.html)
-   [EMEA Localization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157122959910.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
