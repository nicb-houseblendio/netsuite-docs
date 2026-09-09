---
id: "section_N3196172"
type: "section"
title: "Journal Entry"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions-related Records > Journal Entry"
parent: "article_160518507969"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3196172.html"
anchors: ["bridgehead_3909182379", "bridgehead_3909182437", "bridgehead_4544335871", "bridgehead_3999739293"]
sha256: "7b72b5dbc8be497de20e4f86e14a2eefbfb7445cb897207a993ec204c4d0214a"
---

You use the journal entry record to adjust balances in your ledger accounts without entering posting transactions.

In the UI, you access this record in the UI at _Transactions > Financial > Make Journal Entries_.

If your account has the Multi-Book Accounting feature enabled, you can also work with book specific journal entry records, which are available in the UI at _Transactions > Financial > Make Book Specific Journal Entries_. Although they have different entry forms, both book specific and regular intercompany journal entries are the same record type. Within SuiteScript, they are differentiated by the accountingbook field. In other words, a record that has a value set for accountingbook is book specific. Otherwise, the record is a regular intercompany journal entry.

For help working with this record in the UI, see [Making Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475891.html) and [Book-Specific Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3862795782.html#bridgehead_3867000509).

The internal ID for this record is `journalentry`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/journalentry.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_3909182379}

The journal entry record is scriptable in both client SuiteScript and server SuiteScript.

All three user events are supported: beforeLoad, beforeSubmit, and afterSubmit.

## Supported Functions {#bridgehead_3909182437}

The journal entry record is fully scriptable - it can be created, copied, updated, deleted, and searched using SuiteScript.

Warning:

If you update any type of journal entry that has been applied as a payment to an invoice or vendor bill, the relationship between the journal entry and payment is removed and the payment is no longer applied.

## Usage Notes {#bridgehead_4544335871}

With the Advanced Revenue Management (Essentials) feature, you can directly attach a revenue recognition plan to a book specific journal entry or an intercompany journal entry. Before you begin working with advanced revenue management programmatically, see [Setup for Advanced Revenue Management (Essentials)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4328435754.html).

The following table lists the scriptable field associated with this record and advanced revenue management (essentials).

| **Field** | **Type** | **Internal ID** |
| --- | --- | --- |
| End Date | Date | `enddate` |
| Revenue Recognition Rule | List/Record | `revenuerecognitionrule` |
| Start Date | Date | `startdate` |

For help working with this record in the UI, see [Creating Revenue Elements from Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4423536353.html)

## Code Samples {#bridgehead_3999739293}

The following sample shows how to create a book-specific journal entry. The record is book-specific because the parameter `bookje` has been set to `T`.

          `var journalEntry = record.create({     type: record.Type.JOURNAL_ENTRY,     isDynamic: true,     defaultValues: {         bookje: 'T' // Setting bookje parameter to T makes the journal book specific.     } }); journalEntry.setValue({     fieldId: 'accountingbook',     value: '2' }); journalEntry.setValue({     fieldId: 'subsidiary',     value: '4' }); journalEntry.setValue({     fieldId: 'trandate',     value: new Date(2019, 04, 16) }); journalEntry.selectNewLine({     sublistId: 'line' }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'account',     value: '6' }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'credit',     value: '2.00' }); journalEntry.commitLine({     sublistId: 'line' });  journalEntry.selectNewLine({     sublistId: 'line' }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'account',     value: '149' }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'debit',     value: '2.00' }); journalEntry.commitLine({     sublistId: 'line' }); var id = journalEntry.save();` 
        

### Related Topics

-   [Making Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469880.html)
-   [Book-Specific Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3862795782.html#bridgehead_3867000509)
-   [Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1468455.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)
-   [NetSuite Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1379709.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
