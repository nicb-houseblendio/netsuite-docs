---
id: "section_N3201267"
type: "section"
title: "Currency"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Lists > Currency"
parent: "chapter_N3200673"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3201267.html"
anchors: ["bridgehead_1492454071", "bridgehead_1492454126", "bridgehead_1492458975"]
sha256: "c5cf6967d2623ffc1f94c791cc8621a43a0dc96b2e16ed04c69904c957115140"
---

For help working with this record in the UI, see [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html).

The internal ID for this record is `currency`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/currency.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492454071}

The currency record is scriptable in server SuiteScript only.

## Supported Functions {#bridgehead_1492454126}

When the Multiple Currencies feature is enabled, full server scripting is supported for this record type.

When the Multiple Currencies feature is not enabled, scripting does not support create, edit, delete, or search of currency records. Search-based functions such as [search.lookupFields(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345776651.html) are not supported, because search is not supported. Loading of a currency record to get field values is supported if the currency ID is known, as shown in the following sample:

          `var rec = record.load({     type: record.Type.CURRENCY,     id: 1 }); var symbol=rec.getValue({     fieldId: 'symbol' });` 
        

## Usage Notes {#bridgehead_1492458975}

The `currencyprecision` field is available for scripting, even when the ALLOWCURRENCYPRECISIONCHANGE preference is disabled and the field is read-only. In scripting, this field is always a number and never a list, behavior which differs from this field's behavior in the UI.

### Related Topics

-   [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3200673.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
