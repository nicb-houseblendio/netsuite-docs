---
id: "section_N1567137"
type: "section"
title: "Payment Card Number Security and Compliance"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Payment Card Number Security and Compliance"
parent: "section_N1566458"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567137.html"
anchors: ["bridgehead_1544528009", "bridgehead_N1567183", "bridgehead_3887819077"]
sha256: "4a4c367dc8577dd47c732a99abc8895e837587cab68da3b19c1ca0e3e9d523a5"
---

NetSuite is Payment Card Industry Data Security Standard (PCI DSS) level 1 compliant. Therefore, NetSuite may preserve payment card numbers. For information about the PCI DSS, see [https://www.pcisecuritystandards.org](https://www.pcisecuritystandards.org).

Warning:

Only enter and maintain payment card information in secure encrypted fields available in NetSuite on the Payment Instruments or Credit Card subtab of Customer records and on transaction forms (Sales Orders, Cash Sales, Customer Deposits, Customer Payments, Customer Refunds, and Cash Refunds).

Don't enter payment card information in unencrypted fields. Entering payment card information in unencrypted fields violates the PCI Data Security Standard and may lead to payment card data theft. Punitive actions by card associations and your merchant account provider may follow, including financial penalties and a loss of payment card acceptance rights.

With the exception of entering a new card, you can't access unmasked payment card numbers under any role unless a permission is explicitly granted. This security measure protects the customer account data against unauthorized access, fraud, and other security issues.

## Displaying Unencrypted Payment Card Numbers with an Explicit Permission {#bridgehead_1544528009}

To see unmasked payment card numbers, you must log in under a role with the **View Unencrypted Credit Cards** permission. To obtain this permission, an administrator must contact Customer Support and provide a signed agreement. Then, Customer Support activates the View Unencrypted Credit Cards permission for your account. Note that the View Unencrypted Credit Cards permission may only be granted for project work for a period of 90 days.

If you print, send by email, or fax transactions, for example Sales Orders, payment card numbers are not displayed in unmasked form regardless of your permissions. Unmasked payment card numbers are displayed only in the following situation: you have the View Unencrypted Credit Card Numbers permission and you run a saved search that includes payment card numbers in the results.

## Displaying Unmasked Payment Card Number for Administrative Purposes {#bridgehead_N1567183}

Certain business administrative functions require access to full unmasked payment card numbers. According to Visa U.S.A. and the NetSuite PCI auditing service, displaying unmasked payment card numbers in and of itself doesn't fail to meet the PCI Data Security Standard or Visa U.S.A.'s CISP requirements. If you must display full card numbers, ensure that sufficient controls are in place to guarantee the security of the card number data.

The PCI Data Security Standard 4.0.1 provides the following guidelines on masking the Primary Account Number (PAN), with the exception of administrative functions that require the full number:

-   "Requirement 3: concerns protection of stored data; specifically primary account numbers, or PANs, and sensitive authentication data, or SAD, using methods that include hashing truncation, and/or encryption. The main goal of this requirement is to minimize all risks associated with the storage of cardholder data. Mainly, if the data isn't needed, DO NOT STORE IT."
    
-   "3.4 relates to masking PAN numbers when displayed, such as on screens or when printed in reports or receipts. "Masking" involves "hiding" the middle digits of the PAN, so that a maximum of first six and last four digits is all that is displayed. This requirement relates to the protection of PAN numbers displayed on screens, paper receipts, etc., and isn't to be confused with Requirement 3.4 for protection of the PAN when stored in files, databases, etc."
    

## Payment Card Numbers in Search {#bridgehead_3887819077}

To ensure the security of your customers' payment card information, search criteria based on the Credit Card Number field can only use the following operators: **is empty** or **isn't empty**. This includes payment card number searches executed programmatically by using SOAP web services, SuiteScript, or SuiteFlow.

### Related Topics

-   [Accepting Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1569326.html)
-   [Credit Card Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567295.html)
-   _Credit Card Processing Gateway FAQ_
    
-   [Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1566458.html)
-   [Maintaining Recurring Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3887850446.html)
-   [Managing Payment Holds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1570238.html)
-   [Order Verification Rules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567770.html)
-   [Reviewing Payment Status and Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1570238.html#section_N1568265)
-   [Setting Up Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572221.html)
-   [Setting Up Customer Credit Card Soft Descriptors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1568841.html)
-   [Transitioning to a New Gateway and Disabling the Old Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1566955.html#section_N1577424)
-   [Using CyberSource Decision Manager for Fraud Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1492534842.html)
-   [Viewing Customer Credit Card Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1571967.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
