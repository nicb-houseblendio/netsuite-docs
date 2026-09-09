---
id: "chapter_N3739047"
type: "chapter"
title: "Website"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Website"
parent: "book_156388697975"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3739047.html"
anchors: ["bridgehead_N3739057", "bridgehead_N3739088", "bridgehead_N3739315", "bridgehead_N3739352"]
sha256: "9c81d13cce7f3850c303192c0238cfd24af5bbbac55f7a105e7ccef37d328f99"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0220092558.html).

One website record is supported in SOAP web services: Site Category.

To organize information and items for sale on your website, put them in categories. Categories must be associated with presentation tabs for them to display on your website.

For information about working with site categories in the UI, see [Creating Site Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2596427.html).

## Site Category {#bridgehead_N3739057}

The site category record is defined in the [listsWebsite (website)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/website.xsd) XSD.

## Supported Operations {#bridgehead_N3739088}

The following operations can be used with the site category record:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3739315}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [site category](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/sitecategory.html) reference page.

Note:

For information on using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3739352}

Root site categories, such as the Welcome Page, are not editable in SOAP web services because they have negative internalIds. For example, the following update operation fails when submitted:

          `<update xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">   <record internalId="-102" xsi:type="ns1:SiteCategory"    xmlns:ns1="urn:website_2017_1.lists.webservices.netsuite.com">     <ns1:pageTitle xsi:type="xsd:string">pageTitle</ns1:pageTitle>   </record> </update>` 
        

**where:**

internalId="-102" is the internal ID of a root category

If you attempt to edit or update root site categories, the following error message is returned: `Cannot update root level website categories through SOAP web services`.

### Related Topics

-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
