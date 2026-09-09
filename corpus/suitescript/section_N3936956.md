---
id: "section_N3936956"
type: "section"
title: "Tax Group"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Lists > Tax Group"
parent: "chapter_N3200673"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3936956.html"
anchors: ["bridgehead_N3936977", "bridgehead_3733861396", "bridgehead_N3937209"]
sha256: "925a12588d43d0f3f2fbac8f03361e2e4c3de12fbc272a005810653ac83138e2"
---

You can use the tax group record to combine several tax codes, even if the taxes are paid to different jurisdictions. For example, a tax group in the US might include a state tax, a city tax, and a transit tax. The advantage of using a tax group is that, when you create a sales invoice, you can apply one tax group to the transaction, instead of several separate tax codes.

In the UI, you go to this record by choosing _Setup > Accounting > Tax Groups_.

For help working with this record in the UI, see [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html).

The internal ID for this record is `taxgroup`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/taxgroup.html) for the internal IDs of fields, search filters, and search columns associated with this record.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_N3936977}

The tax group record is scriptable in both client SuiteScript and Server SuiteScript.

All three user events are supported: `beforeLoad`, `beforeSubmit`, and `afterSubmit`.

## Supported Functions {#bridgehead_3733861396}

The tax group record is fully scriptable, which means that it can be created, updated, copied, deleted, and searched using SuiteScript.

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html).

## Code Samples {#bridgehead_N3937209}

The following sample shows how to create a US tax group.

          `var initValues = new (); initValues.nexuscountry = 'US';  var taxgroup = record.create({     type: record.Type.TAX_GROUP,     isDynamic: true,     defaultValues: {         'nexuscountry' : 'US'     } }); taxgroup.setValue({     fieldId: 'itemid',     value: 'Test US Tax Group' }); taxgroup.setValue({     fieldId: 'description',     value: 'Tax group description' }); taxgroup.selectNewLine({     sublistId: 'taxitem' }); taxgroup.setCurrentSublistValue({     sublistId: 'taxitem',     fieldId: 'taxname',     value: '-1425'        // -1425 is ID of TX_BUFFALO Tax Code }); taxgroup.commitLine({     sublistId: 'taxitem' });                  recId = taxgroup.save();` 
        

The following code sample shows how to create a tax group for Canada.

          `var newgroup = record.create({     type: record.Type.TAX_GROUP,     defaultValues: {         'nexuscountry': 'CA'     } }); newgroup.setValue({     fieldId: 'itemid',     value: 'CA-T5' }); newgroup.setValue({     fieldId: 'piggyback',     value: 'T' }); newgroup.setValue({     fieldId: 'taxitem1',     value: 21           // Canadian tax code }); newgroup.setValue({     fieldId: 'taxitem2',     value: 24           // Canadian tax code }); newgroup.setValue({     fieldId: 'subsidiary',     value: 2            // Canadian subsidiary }); newgroup.setValue({     fieldId: 'state',     value: 'AB'         // Canadian subsidiary }); newgroup.setValue({     fieldId: 'description',     value: 'New Canada Tax Group' }); var recID = newgroup.save();` 
        

### Related Topics

-   [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3200673.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
