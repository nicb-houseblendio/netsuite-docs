---
id: "section_N3715305"
type: "section"
title: "Download Item"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Items > Download Item"
parent: "chapter_N3704574"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3715305.html"
anchors: ["bridgehead_N3715421", "bridgehead_N3715660", "bridgehead_N3715697", "bridgehead_N3716893", "bridgehead_N28681951", "bridgehead_N28682011", "bridgehead_N28682071"]
sha256: "b3f29273c7a3f6e1cf68de41baf6a4ac58dfadf99f118da1fdd0e21bdfe51adc"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Download Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_60211156500.html).

Create download item records for files you want customers to purchase and download in your Web store. Customers are charged per download item as opposed to per item. For example, if you want to charge customers for music downloads per song, you would create a download item record for each song. If you want to charge customers per album, you would create one download item record and attach each song on the album to the record.

In SOAP web services, the download item record is defined in the [listAcct (accounting)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd) XSD.

Important:

The download item record type is not accessible until the **Sell Download Files** feature is enabled in your account. In SOAP web services an error is thrown if you attempt create, update, delete or search for a Download Item without first enabling the **Sell Download Files** feature. To enable this feature, a NetSuite administrator can go to _Setup > Company > Enable Features_ and select the Items & Inventory subtab, check the Sell Downloadable Files box and click Save.

For general information about the download item record, see these topics in the NetSuite Help Center:

-   [Inventory Management Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2249539.html)
    
-   [Download Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248348.html)
    
-   [Setting Up Items for the Web Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2585301.html#section_N2177433)
    

## Supported Operations {#bridgehead_N3715421}

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [searchMoreWithId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3523074.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3715660}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [download item](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/downloaditem.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3715697}

Please note the following when working with the download items record:

-   The download items record does not have its own search interface. Like all other item types in NetSuite, you must use the [Item Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3713653.html) record to retrieve information for this record type.
    
-   Working with the download item is generally a two-step process. You must first create the download item record using the **add** operation, then you must use the **attach** operation to attach all associated files. Note that an error is thrown if you attempt to attach a file that does not already exist in NetSuite. If you choose, you can later use the **detach** operation to remove a file from a download item record.
    

Note:

You can create both the download item record and file record in one step using the addList operation. However, to attach any file to the download item record, you will still need to call the attach operation.

-   In SOAP web services there is a 10 MB file size limit for file upload. If you attempt to upload a file larger than 10 MB to attach to a download item record, an error is thrown.
    
-   When you do a **get** on download item records, the details of the files attached to the record are not returned in your SOAP response. If you need to get the list of files attached to a download item, you must do an advanced search on the item record and specify the fields on the file record that you want returned. If you want to update the files attached to a download item record, you must update the file record directly.
    
-   To search on the files associated with a download item record, use the file join on the [Item Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3713653.html) record.
    

## Sample Code {#bridgehead_N3716893}

## C# {#bridgehead_N28681951}

          `NetSuiteService nss = new NetSuiteService();            ItemSearchAdvanced itemSearchAdv = new ItemSearchAdvanced();            // Create search criteria          ItemSearch itemSearch = new ItemSearch();          ItemSearchBasic itemSearchBasic = new ItemSearchBasic();            // Set item search type to downloadItem          SearchEnumMultiSelectField itemTypeFld = new SearchEnumMultiSelectField();          String [] itemTypes = new String[1];          itemTypes[0] = "_downloadItem";          itemTypeFld.searchValue = itemTypes;          itemTypeFld.operatorSpecified = true;          itemTypeFld.@operator = SearchEnumMultiSelectFieldOperator.anyOf;          itemSearchBasic.type = itemTypeFld;            // Select search return columns          ItemSearchRow itemRow = new ItemSearchRow();            // Select to return file internal id          FileSearchRowBasic fileRowBasic = new FileSearchRowBasic();            SearchColumnSelectField [] selectColumns = new SearchColumnSelectField[1];          SearchColumnSelectField selectColumn = new SearchColumnSelectField();          selectColumns[0] = selectColumn;          fileRowBasic.internalId = selectColumns;            // Select to return file name          SearchColumnStringField [] stringColumns = new SearchColumnStringField[1];          SearchColumnStringField stringColumn = new SearchColumnStringField();          stringColumns[0] = stringColumn;          fileRowBasic.name = stringColumns;            // Set file join          itemRow.fileJoin = fileRowBasic;                    // Select to return item internalId          ItemSearchRowBasic itemRowBasic = new ItemSearchRowBasic();          itemRowBasic.internalId = selectColumns; // column definition can be reused          itemRow.basic = itemRowBasic;            // Set item search criteria          itemSearch.basic = itemSearchBasic;          itemSearchAdv.criteria = itemSearch;            // Set item return columns          itemSearchAdv.columns = itemRow;            // Perform search          SearchResult searchResult = nss.search(itemSearchAdv);` 
        

## SOAP Request {#bridgehead_N28682011}

          `<search xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <searchRecord xmlns:q1="urn:accounting_2017_1.lists.webservices.netsuite.com" xsi:type="q1:ItemSearchAdvanced">                <q1:criteria>                   <q1:basic>                      <type operator="anyOf" xmlns="urn:common_2017_1.platform.webservices.netsuite.com">                         <searchValue xmlns="urn:core_2017_1.platform.webservices.netsuite.com">_downloadItem</searchValue>                      </type>                   </q1:basic>                </q1:criteria>                <q1:columns>                   <q1:basic>                      <internalId xmlns="urn:common_2017_1.platform.webservices.netsuite.com" />                   </q1:basic>                   <q1:fileJoin>                      <internalId xmlns="urn:common_2017_1.platform.webservices.netsuite.com" />                      <name xmlns="urn:common_2017_1.platform.webservices.netsuite.com" />                   </q1:fileJoin>                </q1:columns>             </searchRecord>          </search>` 
        

## SOAP Response {#bridgehead_N28682071}

          `<platformCore:searchRowList>                   <platformCore:searchRow xsi:type="listAcct:ItemSearchRow" xmlns:listAcct="urn:accounting_2017_1.lists.webservices.netsuite.com">                      <listAcct:basic xmlns:platformCommon="urn:common_2017_1.platform.webservices.netsuite.com">                         <platformCommon:internalId>                            <platformCore:searchValue internalId="105"/>                         </platformCommon:internalId>                      </listAcct:basic>                      <listAcct:fileJoin xmlns:platformCommon="urn:common_2017_1.platform.webservices.netsuite.com">                         <platformCommon:internalId>                            <platformCore:searchValue internalId="239"/>                         </platformCommon:internalId>                         <platformCommon:name>                            <platformCore:searchValue>IDreamedADreamLyrics.txt</platformCore:searchValue>                         </platformCommon:name>                      </listAcct:fileJoin>                   </platformCore:searchRow>                </platformCore:searchRowList>` 
        

### Related Topics

-   [Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3704574.html)
-   [Usage Notes for Item Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705128.html)
-   [Working with Matrix Items in SOAP web services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705423.html)
-   [Shared Field Definitions for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3707811.html)
-   [Item Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3713653.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
