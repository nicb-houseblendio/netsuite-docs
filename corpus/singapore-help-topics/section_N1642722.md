---
id: "section_N1642722"
type: "section"
title: "Singapore Payment Formats"
branch: "singapore-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Singapore Help Topics > Singapore Payment Formats"
parent: "section_4256391369"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1642722.html"
anchors: []
sha256: "1b2d667f20fffbf4b83d34e5f2d7651c49e54070ef250db1ff1b0c5a5f52ca52"
---

You must install the Electronic Bank Payments SuiteApp and Southeast Asia Localization SuiteApp to set up and specify Singapore electronic payment file formats as the electronic fund transfer (EFT) or direct debit templates.

The following table lists the Singapore payment file formats, payment format type, and which SuiteApp you can get them from.

| Singapore electronic payment file format | Payment format type | SuiteApp you must install |
| --- | --- | --- |
| DBS - IDEAL specifications of DBS Bank Limited | electronic fund transfer | Electronic Bank Payments SuiteApp |
| DBS Singapore Ideal 3.0 Universal File Format Domestic Transfer | electronic fund transfer | Southeast Asia Localization SuiteApp |
| DBS Singapore Ideal 3.0 Universal File Format International Transfer | electronic fund transfer | Southeast Asia Localization SuiteApp |
| UoB - BIB-IBG specifications of United Overseas Bank Limited | electronic fund transfer | Electronic Bank Payments SuiteApp |
| ISO 20022 of HSBC | electronic fund transfer | Electronic Bank Payments SuiteApp |
| Citibank Singapore XML Domestic Transfer | electronic fund transfer | Southeast Asia Localization SuiteApp |
| Citibank Singapore XML International Transfer | electronic fund transfer | Southeast Asia Localization SuiteApp |
| Citibank Singapore XML GIRO | electronic fund transfer | Southeast Asia Localization SuiteApp |
| HSBC Singapore pain.001.001.03 Low and High Value Domestic Payments | electronic fund transfer | Southeast Asia Localization SuiteApp |
| JP Morgan Singapore pain.001.001.03 Low and High Value Domestic Payments | electronic fund transfer | Southeast Asia Localization SuiteApp |
| OCBC Singapore GIRO and FAST Payments | electronic fund transfer | Southeast Asia Localization SuiteApp |
| Standard Chartered Bank Singapore iPayment CSV GIRO and Domestic Payments | electronic fund transfer | Southeast Asia Localization SuiteApp |
| UOB Singapore pain.001.001.03 GIRO, FAST and Domestic Payments | electronic fund transfer | Southeast Asia Localization SuiteApp |
| DBS - IDEAL DD (DBS Bank) | direct debit | Electronic Bank Payments SuiteApp |
| UoB - BIB-IBG DD (United Overseas Bank) | direct debit | Electronic Bank Payments SuiteApp |

Note:

To use international transfer payment formats, you must have an active license for advanced Electronic Bank Payments, and you must install the NetSuite SuiteApps License Client SuiteApp in your account. With an active license for advanced Electronic Bank Payments, domestic and cross-border templates are available and you can edit the template as needed. If you use the free version of Electronic Bank Payments, only domestic templates are available and you can't edit the template, but you can edit the PFA output file.

Singapore payment formats contain the required information for electronic fund transfers when paying sales order, vendor bills, vendor credits, employee expenses, refunding customers or compensating partners within Singapore and abroad.

To use these payment formats, you must install or update the Electronic Bank Payments SuiteApp first, followed by installation or update of the Southeast Asia Localization SuiteApp. If you do so, the Southeast Asia Localization SuiteApp adds the Singapore payment formats in the Electronic Bank Payments SuiteApp.

For more information about installing the required SuiteApps, see [Setting Up Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3831186542.html) and [Installing the Southeast Asia Localization SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1523861295.html).

The following table provides the actions you can take in given scenarios to get the Singapore payment formats from the Southeast Asia Localization SuiteApp and add them in the Electronic Bank Payments SuiteApp.

| Scenario | Actions |
| --- | --- |
| Southeast Asia Localization SuiteApp and Electronic Bank Payments SuiteApp are not yet installed | 
1.  Install the latest version of Electronic Bank Payments SuiteApp.
2.  Install the latest version of Southeast Asia Localization SuiteApp.
3.  If successful, open the Electronic Bank Payments SuiteApp and go to Payments > Setup > Payment File Formats, where the Singapore payment formats should be listed.

 |
| Southeast Asia Localization SuiteApp is already installed, but not the Electronic Bank Payments SuiteApp | 

1.  Install the latest version of Electronic Bank Payments SuiteApp.
2.  Update Southeast Asia Localization SuiteApp to the latest version.
3.  If successful, open the Electronic Bank Payments SuiteApp and go to Payments > Setup > Payment File Formats, where the Singapore payment formats should be listed.

 |
| Electronic Bank Payments SuiteApp is already installed, but not the Southeast Asia Localization SuiteApp | 

1.  Update Electronic Bank Payments SuiteApp to the latest version.
2.  Install the latest version of Southeast Asia Localization SuiteApp.
3.  If successful, open the Electronic Bank Payments SuiteApp and go to Payments > Setup > Payment File Formats, where the Singapore payment formats should be listed.

 |
| Both Southeast Asia Localization SuiteApp and Electronic Bank Payments SuiteApp are already installed | 

1.  Update Electronic Bank Payments SuiteApp to the latest version.
2.  Update Southeast Asia Localization SuiteApp to the latest version.
3.  If successful, open the Electronic Bank Payments SuiteApp and go to Payments > Setup > Payment File Formats, where the Singapore payment formats should be listed.

 |

To set up the Electronic Bank Payments SuiteApp for your company, subsidiaries, vendors, employees, customers, and partners in the Singapore, read the following topics:

-   [Setting Up Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3831186542.html)
    
-   [Payment File Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1675118.html)
    
-   [Setting Up Company Bank Records in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1645419.html)
    
-   [Setting Up Bank Records of Vendors in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1646764.html)
    
-   [Setting Up Bank Records of Employees in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1647136.html)
    
-   [Setting Up Bank Records of Customers in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1647643.html)
    
-   [Setting Up Bank Records of Partners in Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851239814.html)
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
