---
id: "section_N3658677"
type: "section"
title: "Usage Notes for Transaction Record Types"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Usage Notes for Transaction Record Types"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3658677.html"
anchors: []
sha256: "fcb49d62a252f9c36f5a11c3a32a86edc6ef5082e18ff0673c4ad81de9f75dfc"
---

Note the following when working with transactions:

-   To maintain performance, 5,000 lines per transaction is the maximum limit for transactions submitted through synchronous and asynchronous SOAP web services. For journal entries, the limit is 1,000 lines for synchronous SOAP web services. With asynchronous SOAP web services, the limit for journal entries is 10,000 lines.
    
    Note:
    
    The 5000 lines per transaction limit for synchronous and asynchronous SOAP web services is the maximum limit under favorable conditions. If your request has less than 5000 lines, but still times out after 6 minutes, break it down into smaller chunks to improve performance.
    
-   There is a 200 record limit for SOAP web services transactions.
    
-   If you have the Multiple Shipping Routes (MSR) feature turned on in your NetSuite account, and you want to enabled MSR on a specific transaction, see [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html).
    
-   The _rate_ field on a sublist can be set without explicitly setting price level to **custom**. Even though NetSuite does not treat the price level as required to set the rate field, users should set the item price level to "-1" (custom) at the time they are setting the item rate.
    
-   The 2011.2 and later endpoints include a change from previous endpoints to the currency field in the body of transactions. Endpoints prior to 2011.2 included the **currencyName** string type field. As of the 2011.2 endpoint, this field has been replaced by the **currency** RecordRef type field. If you upgrade to the 2011.2 endpoint or later, you must update any code that references **currencyName.**
    
-   In the 2012.1 and later endpoints, you can set the currency value for some newly created transactions when the Multiple Currencies feature is enabled. These edits is supported for the following transactions: Cash Refund, Cash Sale, Credit Memo, Customer Deposit, Customer Payment, Customer Refund, Esitmate, Invoice, Item Receipt, Opportunity, Purchase Order, Return Authorization, Sales Order, Vendor Bill, Vendor Credit, Vendor Payment, Vendor Return Authorization. (You cannot edit this value in earlier endpoints.) The currency value for a transaction must be one of the currencies defined for the transaction's customer in the CustomerCurrencyList. See [Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639940.html) and [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).
    

### Related Topics

-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Transaction Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659492.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
