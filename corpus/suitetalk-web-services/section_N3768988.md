---
id: "section_N3768988"
type: "section"
title: "Custom Record"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Customization > Custom Record"
parent: "chapter_N3768661"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3768988.html"
anchors: ["bridgehead_N3769008", "bridgehead_N3769232", "bridgehead_N3769270", "bridgehead_3987720012", "bridgehead_3987720441", "bridgehead_3823604130", "bridgehead_1491316092", "bridgehead_N28967321", "bridgehead_N28967471"]
sha256: "54c3f0ca9d1d54fa59dbdf56b844144df158645c06346a697f1a2c3dcd54cb7f"
---

Custom records are entry forms based on existing record types, but customized to include fields for gathering information specific to the needs of your business. Use the custom record object to define records to emulate existing custom records.

For information about working with this record in the UI, see [Custom Records Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2875173.html).

The custom record object is defined in the [setupCustom (customization)](https://webservices.netsuite.com/xsd/setup/v2025_2_0/customization.xsd) XSD.

## Supported Operations {#bridgehead_N3769008}

The following operations can be used with the custom record record type.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3769232}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [custom record](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/customrecord.html) reference page.

Note:

If you are using the 2013.2 WSDL or later, you may notice that this record's Translations sublist is exposed. However, this sublist is available only in certain cases. Specifically, for the Translations sublist to be available, the corresponding record type must have the enableNameTranslation field set to a value of True. For more details on configuring a record type so that it allows for translations, see [Translating Custom Record Instance Names](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3746164319.html). For details on working with custom record types through SOAP web services, see [Custom Record Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3769505.html).

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3769270}

Currently NetSuite does not support the **store values** option on custom records. Additionally, see the following:

-   [Using CustomRecordRef](#bridgehead_3987720012)
    
-   [Understanding altName and autoName](#bridgehead_3987720441)
    

## Using CustomRecordRef {#bridgehead_3987720012}

Further, note that when referencing custom records, you may need a separate CustomRecordRef type and a RecordRef type.

RecordRef and CustomRecordRef both descend from BaseRef. They are most prominently used in **get()**, and that is why they have a type attribute. CustomRecordRef has a typeId to indicate which **kind** of CustomRecord it is. Therefore, you cannot get a CustomRecord by setting the RecordRef.type to customRecord on add - you must use CustomRecordRef to specify the kind of CustomRecord.

Note:

For a list of the possible typeIds (or record internalIds), refer to [ListOrRecordRef](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452954.html#bridgehead_N3455299) in the NetSuite Help Center.

CustomRecord descends from Record, like Customer or Opportunity. This is what you submit to **add()** and it is what is returned through search(). CustomRecord uses a RecordRef() to store its type information.

## Understanding altName and autoName {#bridgehead_3987720441}

The altName and autoName fields are available only when you are creating a custom record based on a custom record type configured to use auto-generated numbering. (To check whether a custom record type is configured this way, look at the Enable box on the custom record type's Numbering subtab.)

When you use this sort of custom record type as the basis for a new custom record, the altName field is required on the new custom record form. altName is a string field that represents a label you give the custom record, to be used in the list view. Be aware that the altName field maps to the field labeled Name in the user interface (which is different from the way the field names map when auto-generated numbers are not being used).

In this situation, the SOAP web services field called name maps to the field labeled ID in the user interface. This field represents the auto-generated string assigned to the custom record.

The ID field is labeled **name** in SOAP web services.

The Name field is labeled **altName** in SOAP web services.

In some cases, a custom record type may be set up with both the Enable and Allow Override boxes selected. In these cases, you have the additional option of using the boolean autoName field. The autoName field maps to the box labeled Auto in the user interface. This field lets you disable auto-generated numbering for your new custom record. If you set autoName to false, you must provide a value for the name field (which, again, in the user interface is labeled ID). Note that in this situation, altName is also still required.

The Auto box is labeled **autoName** in SOAP web services.

The ID field is labeled **name** in SOAP web services. This field is read only if the autoName value is true.

The Name field is labeled **altName** in SOAP web services.

## Code Samples {#bridgehead_3823604130}

## SOAP {#bridgehead_1491316092}

Request to get a custom record:

          `<soapenv:Body> <get xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <baseRef internalId="102" typeId="139" xsi:type="ns6:CustomRecordRef" xmlns:ns6="urn:core_2017_1.platform.webservices.netsuite.com"/> </get> </soapenv:Body>` 
        

SOAP response:

          `<soapenv:Body> <getResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <readResponse> <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/> <record internalId="102" xsi:type="setupCustom:CustomRecord" xmlns:setupCustom="urn:customization_2017_1.setup.webservices.netsuite.com"> <setupCustom:isInactive>false</setupCustom:isInactive> <setupCustom:name>Truman Capote</setupCustom:name> <setupCustom:owner internalId="79" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"> <platformCore:name>Tom Smith</platformCore:name> </setupCustom:owner> <setupCustom:recType internalId="139" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"> <platformCore:name>Author page</platformCore:name> </setupCustom:recType> <setupCustom:customFieldList xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"> <platformCore:customField internalId="424" scriptId="custrecord_award_winner" xsi:type="platformCore:BooleanCustomFieldRef"> <platformCore:value>false</platformCore:value> </platformCore:customField> </setupCustom:customFieldList> </record> </readResponse> </getResponse> </soapenv:Body>` 
        

Request to add a custom record:

          `<soapenv:Body> <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <record xsi:type="ns6:CustomRecord" xmlns:ns6="urn:customization_2017_1.setup.webservices.netsuite.com"> <ns6:name xsi:type="xsd:string">Shirley Jackson</ns6:name> <ns6:recType internalId="139" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"> <ns7:name xsi:type="xsd:string">Author page</ns7:name> </ns6:recType> </record> </add> </soapenv:Body>` 
        

SOAP response:

          `<soapenv:Body> <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <writeResponse> <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/> <baseRef internalId="202" typeId="139" xsi:type="platformCore:CustomRecordRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/> </writeResponse> </addResponse> </soapenv:Body>` 
        

The following request searches for custom records.

Important:

When you use a CustomRecordSearch, you must explicitly specify the custom record type in the request, either as a custom transaction (customTransactionType) or a custom record (customRecordType).

          `<soapenv:Body> <search xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <searchRecord xsi:type="ns7:CustomRecordSearchBasic" xmlns:ns7="urn:common_2017_1.platform.webservices.netsuite.com"> <ns7:recType scriptId="customrecord_cr_test" type="customRecordType" xsi:type="ns8:CustomizationRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/> </searchRecord> </search> </soapenv:Body>` 
        

SOAP response:

          `<soapenv:Body> <searchResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <platformCore:searchResult xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"> <platformCore:status isSuccess="true"/> <platformCore:totalRecords>1</platformCore:totalRecords> <platformCore:pageSize>1000</platformCore:pageSize> <platformCore:totalPages>1</platformCore:totalPages> <platformCore:pageIndex>1</platformCore:pageIndex> <platformCore:searchId>WEBSERVICES_3604360_012220184986386871927648213_3ed8496b7685</platformCore:searchId> <platformCore:recordList> <platformCore:record internalId="1" xsi:type="setupCustom:CustomRecord" xmlns:setupCustom="urn:customization_2017_1.setup.webservices.netsuite.com"> <setupCustom:isInactive>false</setupCustom:isInactive> <setupCustom:name>Test_Record1</setupCustom:name> <setupCustom:owner internalId="79"> <platformCore:name>Tom Pober</platformCore:name> </setupCustom:owner> <setupCustom:recType internalId="43"> <platformCore:name>CR_Test</platformCore:name> </setupCustom:recType> </platformCore:record> </platformCore:recordList> </platformCore:searchResult> </searchResponse> </soapenv:Body>` 
        

## Java {#bridgehead_N28967321}

To add a custom record:

          `CustomRecord myCR = new CustomRecord();    RecordRef rt = new RecordRef();    rt.setName("Authors");    rt.setId("3"); // This indicates a typeId of 3 and corresponds to the Authors CustomRecord type    myCR.setRecType(rt);     myCR.setName("Ernest Hemmingway"); // This is what will show up in List->    CustomRecords->Authors under Name    myCR.setCustomFieldList(myCFL); // An already filled out CustomField List    WriteResponse wr = port.add(myCR);` 
        

Note that setTypeId is not submitted since this is the internal ID returned by the response, like for normal records.

To get a custom record:

          `CustomRecordRef customRec = new CustomRecordRef(); customRec.setTypeId("21"); // internal id of the custom record type customRec.setInternalId("1"); // internal id of the custom record entry sessMgr.getWrappedPort().get(customRec, this);` 
        

The following code retrieves the entire custom list for a list with an internal ID of **1**.

          `CustomRecordSearch customRecordSearch = new CustomRecordSearch(); RecordRef recordRef = new RecordRef(); recordRef.setInternalId("1"); customRecordSearch.setRecType(recordRef); SearchResult result = port.search(customRecordSearch);` 
        

## C# {#bridgehead_N28967471}

To add a custom record:

          `CustomRecord myCR = new CustomRecord();     RecordRef rt = new RecordRef();     rt.name = "Authors";     // This indicates a typeId of 3 and corresponds to the Authors CustomRecord type     rt.internalId = "3";     customRecord.recType = rt;     // This is what will show up in List->CustomRecords->Authors under Name     customRecord.name = "Ernest Hemingway";     customRecord.customFieldList = myCFL; // An already filled out CustomField List     WriteResponse wr = port.add(customRecord);` 
        

To get a custom record:

          `CustomRecordRef myCRR = new CustomRecordRef();     myCRR.internalId = "1200"; // The key we got back     myCRR.typeId = "3"; // For Authors     ReadResponse rr = _service.get(myCRR);` 
        

### Related Topics

-   [Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3768661.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
