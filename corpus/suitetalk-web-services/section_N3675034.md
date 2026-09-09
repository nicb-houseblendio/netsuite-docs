---
id: "section_N3675034"
type: "section"
title: "Intercompany Journal Entry"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions-related Records > Intercompany Journal Entry"
parent: "article_160526452785"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3675034.html"
anchors: []
sha256: "6c3667b2940151231ee330a2c17a8295212284fc81a695d80705d3e8ff17ba0e"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Intercompany Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0902090936.html).

An intercompany journal entry record is a specialized type of record available only in OneWorld accounts. An intercompany journal entry records debits and credits to be posted to ledger accounts for transactions between two subsidiaries. In an account that has the Multi-Book Accounting feature enabled, you can also use this record type to create book specific intercompany journal entries.

In the user interface, you access this record as follows:

-   **Intercompany journal entries** - Go to _Transactions > Financial > Make Intercompany Journal Entries_. For help working with this record in the user interface, see [Making Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475891.html).
    
-   **Book specific intercompany journal entries** - Go to _Transactions > Financial > Make Book Specific Intercompany Journal Entries_. Note that this form is available only to accounts that use Multi-Book Accounting. For help working with this record in the user interface, see [Intercompany Journal Entries in Multi-Book Accounting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3867050970.html).
    

The intercompany journal entry record is defined in the [tranGeneral](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/general.xsd) XSD, where it is called InterCompanyJournalEntry.

For more information about using SOAP web services to work with the intercompany journal entry record, see the following sections:

-   [Intercompany Journal Entry Supported Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4105132614.html)
    
-   [Intercompany Journal Entry Body and Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4105132538.html)
    
-   [Intercompany Journal Entry Code Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4105132444.html)
    
-   [Common Errors With Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4105316538.html)
    

### Related Topics

-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Usage Notes for Transaction Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3658677.html)
-   [Transaction Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659492.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
