---
id: "chapter_N3169369"
type: "chapter"
title: "Working with the SuiteScript Records Browser"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > Working with the SuiteScript Records Browser"
parent: "book_14946590423"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html"
anchors: []
sha256: "be679bcca613ad6361964e98c59e983aa8779b2cd599d154dea69fab8fdbe6e7"
---

To access the SuiteScript Records Browser, use the following link:

**[Go to the SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/index.html)**

Important:

When writing SuiteScript, you must use the IDs listed in the NetSuite Help Center. You can access IDs by viewing a NetSuite record's page source, but not all IDs in the source code are supported in SuiteScript. If you create a script that references an unsupported or undocumented ID, and NetSuite later changes the ID, your script may break.

Not all fields in the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/index.html) can be set using SuiteScript. Some fields are read only. Check the NetSuite UI to see if a field can be set. Generally, if you can set a field in the UI, you can set it using SuiteScript. If you cannot set a field in the UI, you cannot set it using SuiteScript. However, you can still get the field's value using SuiteScript.

The [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/index.html) provides a summary of all records, fields, sublists, search joins, search filters, search columns, and record transformations that are supported in SuiteScript. Information about elements is displayed as a series of tables.

To find SuiteScript-supported records and IDs:

1.  Open the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/index.html).
    
    Only records that officially support SuiteScript are listed in the SuiteScript Records Browser.
    
2.  Click the record you want to reference in SuiteScript.
    
    All IDs currently supported for the record are listed.
    

The following table provides examples of objects and methods that use each type of ID:

| ID Type | Object Examples | Method Examples |
| --- | --- | --- |
| Field IDs | 
-   [serverWidget.Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4325837128.html)
-   [record.Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4435738444.html)
-   [record.Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4205869719.html)
-   [currentRecord.CurrentRecord](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4642657958.html)

 | 

-   [Record.getField(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4273153320.html)
-   [CurrentRecord.getField(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4637585044.html)
-   [Record.setValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4273155868.html)
-   [CurrentRecord.setValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4637577499.html)
-   [record.submitFields(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267283788.html)
-   [search.lookupFields(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345776651.html)

 |
| Sublist and sublist field IDs | 

-   [serverWidget.Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4325844858.html)

 | 

-   [Record.commitLine(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4273168899.html)
-   [CurrentRecord.commitLine(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4637565703.html)
-   [Record.getCurrentSublistValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4273170578.html)
-   [CurrentRecord.getCurrentSublistValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4637585213.html)
-   [Record.insertLine(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4273158210.html)
-   [CurrentRecord.insertLine(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4637581252.html)
-   [Record.setSublistValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4273166777.html)

 |
| Search join, filter, and column IDs | 

-   [search.Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4392315904.html)
-   [search.Filter](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345767603.html)
-   [search.Column](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345767216.html)
-   [search.Result](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345767112.html)
-   [search.ResultSet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345767679.html)

 | 

-   [search.create(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345171487.html)
-   [search.load(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345775360.html)
-   [search.createFilter(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345777107.html)
-   [search.createColumn(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345776927.html)

 |
| Transformation IDs | 

-   [record.Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4205869719.html)

 | 

-   [record.transform(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258715.html)

 |

As you use the SuiteScript Records Browser, consider the following:

-   You can use the Records Browser online, or you can download it. For more information, see [Downloading the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157850690634.html#subsect_157850694569).
    
-   For information about governance applied to individual SuiteScript APIs, and about various SuiteScript script types, see [SuiteScript Governance and Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3350651.html).
    
-   Only the Records Browser for the most recent release of NetSuite is supported. Older versions may still be accessible, but they are not supported.
    
-   Green highlighting indicates anything new in the current release.
    

For more details, see the following topics:

-   [Finding a Record or Subrecord](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157850914989.html)
    
-   [SuiteScript Record Summary Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157850915666.html)
    
-   [Deleted Record Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157850916103.html)
    

### Related Topics

-   [SuiteScript Records Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_1494659042.html)
-   [SuiteScript Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163726005075.html)
-   [Setting Up Your SuiteScript Environment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2903520.html)
-   [SuiteScript Governance and Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3350651.html)
-   [SuiteScript Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/part_N3360914.html)
-   [SuiteScript Debugger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3014215.html)
-   [SuiteCloud Processors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1498571420.html)
-   [SuiteScript Monitoring, Auditing, and Logging](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1494642209.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [SuiteScript IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1494647249.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
