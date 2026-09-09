---
id: "section_N3718140"
type: "section"
title: "Item Group"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Items > Item Group"
parent: "chapter_N3704574"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3718140.html"
anchors: ["bridgehead_N3718157", "bridgehead_N3718381", "bridgehead_N3718419", "bridgehead_3820196553", "bridgehead_N28690451", "bridgehead_N28690331", "bridgehead_N28690391"]
sha256: "a6164966c26e6eac85fd0c8f5c059e59d4a6c8145f7d09f514f1df4fa93be243"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Item Group](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0120112015.html).

An item group is stocked and sold as a single unit, but are made up of several individual items.

The item group record is defined in the [listAcct (accounting)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd) XSD.

For information about using this record in the UI, see [Item Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2224824.html).

## Supported Operations {#bridgehead_N3718157}

The following operations can be used with the item group record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3718381}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [item group](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/itemgroup.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3718419}

The following sample shows how to add an item group through SOAP web services. Note that the itemMemberList (Components) sublist is a non-keyed sublist.

## Code Sample {#bridgehead_3820196553}

## Java {#bridgehead_N28690451}

          `public void addItemGroup() throws Exception    {       this.login();         ItemGroup ig = new ItemGroup();         ig.setItemId("Test Item Group");       ig.setDisplayName("Test IG");         //Create a list of subsidiaries       RecordRefList recordRefList = new RecordRefList();       RecordRef rr = new RecordRef();       rr.setInternalId("3");       rr.setType(RecordType.subsidiary);       recordRefList.setRecordRef(new RecordRef[]{rr});       ig.setSubsidiaryList(recordRefList);         RecordRef depRef = new RecordRef();       depRef.setInternalId("2");       ig.setDepartment(depRef);       RecordRef locRef = new RecordRef();       locRef.setInternalId("2");       ig.setLocation(locRef);       RecordRef classRef = new RecordRef();       classRef.setInternalId("2");       ig.set_class(classRef);         //Item sublist       ItemMemberList iml = new ItemMemberList();       ItemMember im = new ItemMember();       RecordRef itRef = new RecordRef();       itRef.setInternalId("39");       im.setItem(itRef);       im.setQuantity(3.0);       im.setVsoeDeferral(VsoeDeferral._deferUntilItemDelivered);       im.setVsoeDelivered(true);       im.setVsoePermitDiscount(VsoePermitDiscount._never);       iml.setItemMember(new ItemMember[]{im});         ig.setMemberList(iml);       ig.setDescription("This is a test Item Group");       ig.setIsVsoeBundle(false);       ig.setAvailableToPartners(true);         _port.add(ig);    }` 
        

## SOAP Request {#bridgehead_N28690331}

          `<soapenv:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">     <soapenv:Header>         <ns1:passport soapenv:mustUnderstand="0" soapenv:actor="http://schemas.xmlsoap.org/soap/actor/next" xmlns:ns1="urn:messages_2017_1.platform.webservices.netsuite.com">             <ns2:email xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com">email@netsuite.com</ns2:email>             <ns3:password xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com">*******</ns3:password>             <ns4:account xmlns:ns4="urn:core_2017_1.platform.webservices.netsuite.com">1234567</ns4:account>             <ns5:role internalId="37" xmlns:ns5="urn:core_2017_1.platform.webservices.netsuite.com"/>         </ns1:passport>     </soapenv:Header>     <soapenv:Body>         <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <record xsi:type="ns6:ItemGroup" xmlns:ns6="urn:accounting_2017_1.lists.webservices.netsuite.com">                 <ns6:isVsoeBundle xsi:type="xsd:boolean">false</ns6:isVsoeBundle>                 <ns6:availableToPartners xsi:type="xsd:boolean">true</ns6:availableToPartners>                 <ns6:itemId xsi:type="xsd:string">Test Item Group</ns6:itemId>                 <ns6:displayName xsi:type="xsd:string">Test IG</ns6:displayName>                 <ns6:description xsi:type="xsd:string">This is a test Item Group</ns6:description>                 <ns6:subsidiaryList xsi:type="ns7:RecordRefList" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com">                     <ns7:recordRef xsi:type="ns7:RecordRef" type="subsidiary" internalId="3"/>                 </ns6:subsidiaryList>                 <ns6:department xsi:type="ns8:RecordRef" internalId="2" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <ns6:class xsi:type="ns9:RecordRef" internalId="2" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <ns6:location xsi:type="ns10:RecordRef" internalId="2" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <ns6:memberList xsi:type="ns6:ItemMemberList" replaceAll="false">                     <ns6:itemMember xsi:type="ns6:ItemMember">                         <ns6:quantity xsi:type="xsd:double">3.0</ns6:quantity>                         <ns6:vsoeDeferral xsi:type="ns11:VsoeDeferral" xmlns:ns11="urn:types.common_2017_1.platform.webservices.netsuite.com">_deferUntilItemDelivered</ns6:vsoeDeferral>                         <ns6:vsoePermitDiscount xsi:type="ns12:VsoePermitDiscount" xmlns:ns12="urn:types.common_2017_1.platform.webservices.netsuite.com">_never</ns6:vsoePermitDiscount>                         <ns6:vsoeDelivered xsi:type="xsd:boolean">true</ns6:vsoeDelivered>                         <ns6:item xsi:type="ns13:RecordRef" internalId="39" xmlns:ns13="urn:core_2017_1.platform.webservices.netsuite.com"/>                     </ns6:itemMember>                 </ns6:memberList>             </record>         </add>     </soapenv:Body> </soapenv:Envelope>` 
        

## SOAP Response {#bridgehead_N28690391}

          `<soapenv:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">     <soapenv:Header>         <platformMsgs:documentInfo xmlns:platformMsgs="urn:messages_2017_1.platform.webservices.netsuite.com">             <platformMsgs:nsId>WEBSERVICES_1234567_08102012262722597610660420_af57ceedff97e</platformMsgs:nsId>         </platformMsgs:documentInfo>     </soapenv:Header>     <soapenv:Body>         <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <writeResponse>                 <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <baseRef xsi:type="platformCore:RecordRef" type="itemGroup" internalId="204" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>             </writeResponse>         </addResponse>     </soapenv:Body> </soapenv:Envelope>` 
        

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
