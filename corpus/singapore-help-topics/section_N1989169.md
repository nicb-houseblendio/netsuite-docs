---
id: "section_N1989169"
type: "section"
title: "Singapore Tax Audit File"
branch: "singapore-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Singapore Help Topics > Singapore Tax Topics for Accounts Without SuiteTax > Singapore Tax Audit File"
parent: "chapter_N1981261"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1989169.html"
anchors: []
sha256: "9e97c9630053ed9045493826e04a8d7a89163fbf5c04596523bc90efc6915765"
---

If you have a Singapore subsidiary and nexus, and the Tax Audit Files SuiteApp is installed in your NetSuite account, you can generate the IRAS Audit File (IAF). You can generate the file in either text or XML format.

Important:

You must install the International Tax Reports and Supplementary Tax Calculation SuiteApps to generate Customer Accounting transactions through the Singapore IRAS Audit File (IAF).

NetSuite generates the IAF from data entries in your General Ledger or Chart of Accounts, master data of customers and suppliers, and details of invoices, orders, payments, and adjustments.

![An example of Singapore Audit Files.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/CountrySpecificFeatures/SingaporeTaxAuditFile.png)

Important:

By using the Tax Audit Files SuiteApp, you assume all responsibility for determining whether the data you generate and download is accurate or sufficient for your purposes. You also assume all responsibility for the security of any data that you download from NetSuite and subsequently store outside of the NetSuite system.

To make the generated IAF is compliant with IRAS requirements, you must do the following:

-   For transactions where the Singapore Dollar (SGD) is not the functional currency, make sure the system converts the value of supply and output tax to SGD. Use the prevailing exchange rates for GST reporting purposes.
    
-   Make sure that the Use Account Numbers preference is turned on in _Setup > Accounting > Preferences > Set Up Accounting_.
    
-   Make sure that each posting account has a unique account number in the Chart of Accounts setup. For more information, see [Chart of Account Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440268.html).
    
-   Enter the company's VAT/GST Registration No. and UEN on the company information or Singapore subsidiary record. If you do not have a OneWorld account, go to Setup > Company > Company Information. If you have a OneWorld account, go to Setup > Company > Subsidiaries and select the Singapore subsidiary.
    
-   Provide values for all the required data elements or fields, including:
    
    -   UEN field on customer, partner, and vendor records. This is a custom field that shows when a Singapore subsidiary is selected on an entity record. For information, see [Tracking the Unique Entity Number](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1986994.html).
        
    -   Import Permit No. field on purchase records that involve the import of goods into Singapore. This is a custom field that shows when a Singapore subsidiary is selected on a purchase transaction form. The import permit number represents the cargo clearance import permit number. It is required for the IRAS Audit File.
        
    -   GST Reference Number (Tax Registration Number) on entity records
        
-   Provide details in the transaction memo field of each transaction.
    
-   You should specifying a document date for each transaction you create. The Document Date field determines the date stated in documents such as invoice or vendor bill.
    

To use the Singapore tax audit file, see [Using Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077183.html).

### Related Topics

-   [Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2073244.html)
-   [Prerequisites for Installing the Tax Audit Files SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_98164624128.html)
-   [Installing the Tax Audit Files SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2074100.html)
-   [Using Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077183.html)
-   [Additional Setup Requirements for Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1981722.html)
-   [Singapore Tax Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983547.html)
-   [Singapore Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983994.html)
-   [Setting Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1813668.html)
-   [Setting Tax Rounding Levels, Methods, and Precision Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1814149.html)
-   [Tracking the Unique Entity Number](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1986994.html)
-   [Accounting for Goods and Services Tax - Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1987208.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
