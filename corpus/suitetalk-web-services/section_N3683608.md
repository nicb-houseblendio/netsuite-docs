---
id: "section_N3683608"
type: "section"
title: "Journal Entry"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions-related Records > Journal Entry"
parent: "article_160526452785"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3683608.html"
anchors: []
sha256: "33a6b172e580d3426bb92b5ac80b3a71a1840ec133b16fd1eac4b0ffb91633d6"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159886587653.html).

You use the journal entry record to adjust balances in accounts. Journal entries let you change the value of any set of accounts without having to enter a posting transaction. In an account that has the Multi-Book Accounting feature enabled, you can also use this record to create book specific journal entries.

In the user interface, you access this record as follows:

-   **Journal entries** - Go to _Transactions > Financial > Make Journal Entries_. For help working with this record in the user interface, see [Making Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469880.html).
    
-   **Book specific journal entries** - Go to _Transactions > Financial > Make Book Specific Journal Entries_. Note that this form is available only for accounts that use Multi-Book Accounting. For help working with this record in the user interface, see [Book-Specific Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3862795782.html#bridgehead_3867000509).
    

The journal entry record is defined in the [tranGeneral](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/general.xsd) XSD, where it is called JournalEntry.

For more information about using SOAP web services to work with the journal entry record, see the following sections:

-   [Journal Entry Supported Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4099131522.html)
    
-   [Journal Entry Body and Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4099136433.html)
    
-   [Journal Entry Code Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4102626680.html)
    
-   [Common Errors With Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4103386138.html)
    

### Related Topics

-   [Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1468455.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Usage Notes for Transaction Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3658677.html)
-   [Transaction Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659492.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
