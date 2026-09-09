---
id: "bridgehead_N3253690"
type: "bridgehead"
title: "Company Information Preferences"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript IDs > Preference Names and IDs > Company Information Preferences"
parent: "chapter_N3251359"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3253690.html"
anchors: []
sha256: "976e3467b3f58426a672bc8eeefe68bb704cd2298e225b7375c19accc3d8796b"
---

The Company Information preferences are available at _Setup > Company > Company Information_.

To interact with these preferences, use the `COMPANY_INFORMATION` value from the [config.Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4256772632.html) enum. All Company Information preference IDs are case-sensitive.

For details about working with the Company Information page in the UI, see [Configuring Company Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N240902.html).

Note:

The Company Information page includes several preferences that are displayed as body fields. These fields are described in the following table.

| Preference Label | Preference Internal ID |
| --- | --- |
| Company Name | companyname |
| Legal Name | legalname |
| Company Logo (Forms) | formlogo |
| Company Logo (Pages) | pagelogo |
| Display Logo Internally | displaylogointernally |
| Web Site | url |
| County/State/Province | state |
| Country | country |
| Return Email Address | email |
| Fax | fax |
| Currency | basecurrency |
| Employer Identification Number (EIN) | employerid |
| SSN or TIN (Social Security Number, Tax ID Number) | taxid |
| First Fiscal Month | fiscalmonth |
| Time Zone | timezone |
| Account ID | companyid |
| Customer Center Login | customersurl |
| These three IDs represent text summaries of the data that exists on the three address subrecords. | mainaddress \_text |
| shippingaddress \_text |
| returnaddress \_text |

The Company Information page also includes gray boxes with the headings Address, Shipping Address, and Return Address. In the UI, you interact with these components by clicking the Edit link next to each box. Clicking any of these links displays a popup window that includes more fields.

To interact with these fields programmatically, you must use subrecord methods to access the fields associated with the Address, Shipping Address, and Return Address blocks. You must first instantiate the appropriate subrecord by using [Record.getSubrecord(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4296709996.html). This method requires one argument: the ID of the subrecord. For the address subrecords on the Company Information page, use the following internal IDs:

-   mainaddress
    
-   shipaddress
    
-   returnaddress
    

After you instantiate the subrecord, you can interact with any of the preferences shown in the following table. These preferences are handled as fields on each subrecord instance.

| Preference Label | Preference Internal ID |
| --- | --- |
| Address1 | addr1 |
| Address2 | addr2 |
| Attention | attention |
| Addressee | addressee |
| Phone | addrphone |
| City | city |
| County/State/Province | state |
| Zip | zip |
| Country | country |

For an example, see [Retrieving a Body Field Address Subrecord Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1496879996.html). For general information about subrecords, see [SuiteScript 2.x Scripting Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4675623115.html).

### Related Topics

-   [Permission Names and IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3236764.html)
-   [General Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3251492.html)
-   [User Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3254790.html)
-   [Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3258805.html)
-   [Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3263666.html)
-   [Manufacturing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_160795960465.html)
-   [Tax Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3263873.html)
-   [Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4695736720.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
