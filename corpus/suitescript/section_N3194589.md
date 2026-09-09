---
id: "section_N3194589"
type: "section"
title: "Intercompany Journal Entry"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions-related Records > Intercompany Journal Entry"
parent: "article_160518507969"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3194589.html"
anchors: ["bridgehead_3998983987", "bridgehead_3998984735", "bridgehead_3999733905"]
sha256: "53de1878dc5822e90ad0128aaa78176b091dd14fd105b9c4071f21395b554379"
---

Intercompany journal entries are a specialized type of journal available specifically for OneWorld. An intercompany journal entry records debits and credits to be posted to ledger accounts for transactions between two subsidiaries. These records adjust the value of any set of accounts without the need for transactions such as invoices and bills.

In the UI, you can access this record at _Transactions > Financial > Make Intercompany Journal Entries_.

If your account has the Multi-Book Accounting feature enabled, you can also work with book specific intercompany journal entry records, which in the UI are available at _Transactions > Financial > Make Book Specific Intercompany Journal Entries_. Although they have different entry forms, both book specific and regular intercompany journal entries are the same record type. Within SuiteScript, they are differentiated by the accountingbook field. In other words, a record that has a value set for accountingbook is book specific. Otherwise, the record is a regular intercompany journal entry.

For help working with this record in the UI, see [Making Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475891.html) and [Book-Specific Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3867050970.html#bridgehead_3867055067).

The internal ID for this record is `intercompanyjournalentry`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/intercompanyjournalentry.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_3998983987}

The intercompany journal entry record is scriptable in both client and server SuiteScript.

All three user events are supported: beforeLoad, beforeSubmit, and afterSubmit.

## Supported Functions {#bridgehead_3998984735}

The intercompany journal entry record is fully scriptable - it can be created, updated, copied, deleted, and searched using SuiteScript.

Warning:

If you update any type of journal entry that has been applied as a payment to an invoice or vendor bill, the relationship between the journal entry and payment is removed and the payment is no longer applied.

## Code Samples {#bridgehead_3999733905}

The following sample shows how to create a book specific intercompany journal entry. The record is book specific because a value has been set for the accountingbook field.

          `var journalEntry = record.create({     type: record.Type.INTER_COMPANY_JOURNAL_ENTRY,     isDynamic: true }); journalEntry.setValue({     fieldId: 'accountingbook',     value: 2                      // Setting a value for this field makes the record book-specific. }); journalEntry.setValue({     fieldId: 'subsidiary',     value: 1 }); journalEntry.setValue({     fieldId: 'tosubsidiary',     value: 3 });  journalEntry.selectNewLine({     sublistId: 'line' }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'linesubsidiary',     value:1 }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'account',     value: 1 }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'credit',     value: '2.00' }); journalEntry.commitLine({     sublistId: 'line' });  journalEntry.selectNewLine({     sublistId: 'line' }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'linesubsidiary',     value: 1 }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'account',     value: 2 }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'debit',     value: '2.00' }); journalEntry.commitLine({     sublistId: 'line' }); journalEntry.selectNewLine({     sublistId: 'line' }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'linesubsidiary',     value: 3 }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'account',     value: 6 }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'credit',     value: '2.00' }); journalEntry.commitLine({     sublistId: 'line' });  journalEntry.selectNewLine({     sublistId: 'line' }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'linesubsidiary',     value: 3 }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'account',     value: 149 }); journalEntry.setCurrentSublistValue({     sublistId: 'line',     fieldId: 'debit',     value: '2.00' }); journalEntry.commitLine({     sublistId: 'line' });  var recordId = journalEntry.save();` 
        

### Related Topics

-   [Making Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475891.html)
-   [Book-Specific Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3867050970.html#bridgehead_3867055067)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)
-   [NetSuite Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1379709.html)
-   [Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1468455.html)
-   [Journal Entries in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475513.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
