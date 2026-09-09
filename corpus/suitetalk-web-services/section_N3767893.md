---
id: "section_N3767893"
type: "section"
title: "Vendor Category"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Other Lists > Vendor Category"
parent: "chapter_N3757146"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3767893.html"
anchors: ["bridgehead_N3767911", "bridgehead_N3768122", "bridgehead_1511362530", "bridgehead_1511362583", "bridgehead_1511362671"]
sha256: "5ec63b262263f657ff088c7e18c604879e4c8b4f6c22f6d886201f30e7c004b7"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Vendor Category](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0821113647.html).

The vendor category record is defined in the [listAcct (accounting)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd) XSD.

## Supported Operations {#bridgehead_N3767911}

The following operations can be used with the vendor category record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3768122}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [vendor](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/vendor.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Sample Code {#bridgehead_1511362530}

The following example shows how to add a vendor category through SOAP web services.

## SOAP Request {#bridgehead_1511362583}

          `<soapenv:Body>            <add xmlns="urn:messages_2017_2.platform.webservices.netsuite.com">                <record xsi:type="ns7:VendorCategory" xmlns:ns7="urn:accounting_2017_2.lists.webservices.netsuite.com">                    <ns7:name xsi:type="xsd:string">Insurance Providers</ns7:name>                    <ns7:isTaxAgency xsi:type="xsd:boolean">false</ns7:isTaxAgency>                    <ns7:isInactive xsi:type="xsd:boolean">false</ns7:isInactive>                </record>            </add>        </soapenv:Body>` 
        

## Java {#bridgehead_1511362671}

          `public void vendorCategory() throws Exception {         VendorCategory vendorCat = new VendorCategory();         vendorCat.setName("Insurance Providers");         vendorCat.setIsInactive(false);         vendorCat.setIsTaxAgency(false);          c.addRecord(vendorCat);     }` 
        

### Related Topics

-   [Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3757146.html)
-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3739470.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
