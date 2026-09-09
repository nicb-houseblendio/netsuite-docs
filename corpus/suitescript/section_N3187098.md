---
id: "section_N3187098"
type: "section"
title: "Partner"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Entities > Partner"
parent: "chapter_N3184398"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3187098.html"
anchors: ["bridgehead_1492095852", "bridgehead_1492095915", "bridgehead_N3187140", "bridgehead_N3187148", "bridgehead_N3187324"]
sha256: "eb941eab44063a7176615e429b1ebc88b825631ca853a454f38f774ebebad3e3"
---

A partner is a company you have a business agreement with who isn't a customer or a vendor.

For help working with this record in the user interface, see [Managing Partners](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1166465.html).

The internal ID for this record is `partner`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/partner.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492095852}

The partner record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492095915}

The partner record is fully scriptable - it can be created, updated, copied, deleted, and searched using SuiteScript. It can also be transformed.

## Usage Notes {#bridgehead_N3187140}

## Notes on Scripting Partner Fields {#bridgehead_N3187148}

The following table provides usage notes for specific fields on this record.

| Field Internal ID | Field UI Label | Note |
| --- | --- | --- |
| **Body Fields** |
| password | Password | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |
| password2 | Confirm Password | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |

## Notes on Scripting Partner Sublists {#bridgehead_N3187324}

You can update the contactaccessroles sublist to provide Partner Center access to contacts. You can provide access to contacts that already exist in NetSuite and that have already been attached to a partner that already exists in NetSuite. The workflow is as follows: 1) Add partner. 2) Add contacts. 3) Attach contacts to partner. 4) Update partner with contact access information.

The fields in this sublist map to the fields on the Access subtab in the UI. These fields include: a field that indicates whether a contact has access to NetSuite, contact name key field, email address used to log in to NetSuite, password used to log in to NetSuite, NetSuite role (Partner Center), and a field that indicates whether the contact should receive a notification email when access changes are made. If this Notify field is set to true, an email is sent.

The Access / contactroles sublist is included in the customer record on the Access subtab. It is an inline editor subtab. The Access / contract roles sublist is related to the Contact / contactroles sublist. For details, see the contactroles sublist in the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/partner.html).

### Related Topics

-   [Managing Partners](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1166465.html)
-   [Creating a Partner Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1166599.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3184398.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
