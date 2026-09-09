---
id: "section_N3205030"
type: "section"
title: "Website Setup"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Website > Website Setup"
parent: "chapter_N3204996"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3205030.html"
anchors: ["bridgehead_1493059398", "bridgehead_1493059444", "bridgehead_N3205085", "bridgehead_N3205106", "bridgehead_N3205158"]
sha256: "b040ee1944ee0d7a39a6a8a73a753e6665758930b01d627f5db19f24346458f5"
---

The internal ID for this record is `website`. In the UI, you can find this record by going to _Commerce > Websites > Website List_.

For help working with this record in the UI, see [Site Builder Web Site Record Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2561820.html).

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/website.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1493059398}

The web site setup record is scriptable in server SuiteScript only.

The web site record is not supported in `beforeLoad` user event scripts.

## Supported Functions {#bridgehead_1493059444}

The web site setup record is fully scriptable. It can be created, copied, updated, deleted, and searched using SuiteScript.

## Usage Notes {#bridgehead_N3205085}

Developers can use SuiteScript with the web site setup record whether they are working in accounts using Site Builder, Commerce web stores, or SCIS.

## Creating a Web Site Setup Record in SuiteScript {#bridgehead_N3205106}

The following code sample shows how to create a SuiteCommerce Web Site Setup record using SuiteScript 2.x:

          `/**  * @NApiVersion 2.x  */   require(['N/record'], function(record) {     var initValues = new Array();     initValues.displayname = "name_of_your_website";     initValues.internalname = "name_of_your_website";           initValues.sitetype = "ADVANCED";      initValues.websitescope = "SUITE_COMMERCE";          var objRec = record.create({         type: record.Type.WEBSITE,         defaultValues: initValues     });            var recId = objRec.save({         enableSourcing: false,         ignoreMandatoryFields: false     }); })` 
        

To set up any other kind of website, the same code is applicable but the `sitetype` and `websitescope` parameters must contain different values. The required values for the different site types are as follows:

| Product | sitetype value | websitescope value |
| --- | --- | --- |
| SuiteCommerce | ADVANCED | SUITE\_COMMERCE |
| SuiteCommerce Advanced | ADVANCED | SUITE\_COMMERCE\_ADVANCED |
| SuiteCommerce In Store | ADVANCED | SUITE\_COMMERCE\_IN\_STORE |
| SuiteCommerce My Account | ADVANCED | SUITE\_COMMERCE\_MY\_ACCOUNT |
| Site Builder | STANDARD | One of the following: FULL\_WEB\_STORE INFO\_CATALOG\_PRICING INFO\_CATALOG INFO\_ONLY For more information about these options, see [Multi-Site Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2562624.html#bridgehead_N2563304). |

Note:

Websitescope field for ADVANCED sites is read-only by default. This means that you cannot modify websitescope for an existing ADVANCED site.

## Setting Values for Web Site Setup Dropdown Fields {#bridgehead_N3205158}

The following table lists the dropdown fields on the Web Site Setup record. When writing SuiteScript, if you are setting the value of a dropdown field, use the IDs listed in the column called Internal IDs for Dropdown Values.

| Subtab | Dropdown Field | UI Labels for Dropdown Values | Internal IDs for Dropdown Values |
| --- | --- | --- | --- |
| **Setup subtab** |
|  | 
-   Web Site Scope
-   (websitescope)

Note: Web Site Scope can be changed only for Site Builder sites. | 

-   Full Web Store
-   Information And Catalog, With Pricing
-   Information And Catalog
-   Information Only

 | 

-   FULL\_WEB\_STORE
-   INFO\_CATALOG\_PRICING
-   INFO\_CATALOG
-   INFO\_ONLY

 |
|  | 

Default Customer Category

(defaultcustomercategory)



 | 

-   Corporate
-   Individual
-   Employee

 | 

-   CORPORATE
-   INDIVIDUAL
-   EMPLOYEE

 |
| **Appearance subtab** - applies only to Site Builder |
|  | 

Web Site Logo Alignment

(websitelogoalign)



 | 

-   Align Left
-   Align Right
-   Align Center

 | 

-   LEFT
-   RIGHT
-   CENTER

 |
|  | 

Page Alignment

(pagealign)



 | 

-   Align Left
-   Align Right
-   Align Center

 | 

-   LEFT
-   RIGHT
-   CENTER

 |
|  | 

Display Order of Cart Items

(cartdisplayorder)



 | 

-   Most Recently Added First
-   Most Recently Added Last

 | 

-   RECENT\_FIRST
-   RECENT\_LAST

 |
| **Upsell subtab** |
|  | 

Items to Upsell

(upsellitems)



 | 

-   Show Related Items First and Upsell Items Next
-   Show Upsell Items First and Related Items Next
-   Show Only Related Items
-   Show Only Upsell Items

 | 

-   RELATED\_FIRST\_UPSELL\_NEXT
-   UPSELL\_FIRST\_RELATED\_NEXT
-   ONLY\_RELATED\_ITEMS
-   ONLY\_UPSELL\_ITEMS

 |
|  | 

Items to Upsell in Cart

(cartupsellitems)



 | 

-   Show Related Items First and Upsell Items Next
-   Show Upsell Items First and Related Items Next
-   Show Only Related Items
-   Show Only Upsell Items

 | 

-   RELATED\_FIRST\_UPSELL\_NEXT
-   UPSELL\_FIRST\_RELATED\_NEXT
-   ONLY\_RELATED\_ITEMS
-   ONLY\_UPSELL\_ITEMS

 |
| **Legacy subtab** - applies only to Site Builder |
|  | 

Site Tab Alignment

(sitetabalignment)



 | 

-   Align Left
-   Align Right
-   Align Center

 | 

-   LEFT
-   RIGHT
-   CENTER

 |
| **Shopping subtab** |
|  | 

Sales Order Type

(salesordertype)



 | 

-   Per Customer Basis

 | 

-   PER\_CUSTOMER

 |

### Related Topics

-   [Site Builder Web Site Record Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2561820.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3204996.html)
-   [CMS Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1496235879.html)
-   [CMS Content Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1498487313.html)
-   [CMS Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1496257171.html)
-   [Commerce Category](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4732712917.html)
-   [Shopping Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4823496109.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
