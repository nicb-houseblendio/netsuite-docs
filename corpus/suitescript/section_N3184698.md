---
id: "section_N3184698"
type: "section"
title: "Customer"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Entities > Customer"
parent: "chapter_N3184398"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3184698.html"
anchors: ["bridgehead_1492029375", "bridgehead_1492029410", "bridgehead_N3184740", "bridgehead_N3184748", "bridgehead_N3185023", "bridgehead_N3185039"]
sha256: "6d97dae2b4790e9913b03980c85bf124ee4ee0ca1d4e2eefb00440d46867777e"
---

Customer records allow you to track all the following types of information about your customers in one place, depending on the features you have enabled.

For help working with this record in the user interface, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).

The internal ID for this record is `customer`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/customer.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492029375}

The customer record is scriptable in both client and server SuiteScript.

Note:

The customer center role does not support scripting capabilities. You must log into a valid account role to write and deploy SuiteScripts.

## Supported Functions {#bridgehead_1492029410}

The customer record is fully scriptable - it can be created, updated, copied, deleted, and searched using SuiteScript. It can also be transformed.

## Usage Notes {#bridgehead_N3184740}

## Notes on Scripting Customer Fields {#bridgehead_N3184748}

The following table provides usage notes for specific fields on this record.

| Field Internal ID | Field UI Label | Note |
| --- | --- | --- |
| **Body Fields** |
| datecreated | Date Created | This is a system-generated field that marks the date the record was created in NetSuite. You cannot change or override this field. Tip: If you need to capture 'date created' information that is not related to the date the record was created in NetSuite, create a custom field and set it to auto-default to today's date. |
| password | Password | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |
| password2 | Confirm Password | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |
| **Search Filters and Search Columns** |
| ccnumber | Credit Card Number | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |

The Multi-Partner Management feature must be enabled in your account for the Partners sublist to appear.

The Access / contactroles sublist is included in the customer record on the Access subtab. It is an inline editor subtab. The Access / contract roles sublist is related to the Contact / contactroles sublist. For details, see the contactroles sublist in the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/customer.html).

The Time Tracking sublist is included with the customer record. It is an inline editor sublist.

Important:

If any case, task, or event record has more than 9500 time entries in the Time Tracking sublist, all cases include a static list of time entries. These static lists are not accessible to scripting. Attempts to script on Time Tracking sublists that are static lists of time entries will not return accurate results.

## Notes on Scripting Customer Sublists {#bridgehead_N3185023}

You can update the contactroles sublist to provide Customer Center access to contacts. You can provide access to contacts that already exist in NetSuite and that have already been attached to a customer that already exists in NetSuite. The workflow is as follows: 1) Add customer. 2) Add contacts. 3) Attach contacts to customer. 4) Update customer with contact access information.

The fields in this sublist map to the fields on the Access subtab in the UI. These fields include: a field that indicates whether a contact has access to NetSuite, contact name key field, email address used to log in to NetSuite, password used to log in to NetSuite, NetSuite role (Customer Center), and a field that indicates whether the contact should receive a notification email when access changes are made. If this Notify field is set to true, an email is sent.

## Transform Types {#bridgehead_N3185039}

In the NetSuite Help Center, see [record.transform(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258715.html) for examples on how to transform records.

| Target Record Type | Target Record Internal ID | Field Defaults |
| --- | --- | --- |
| Cash Sale | cashsale | billdate |
| Customer Payment | customerpayment | \- |
| Quote | estimate | \- |
| Invoice | invoice | billdate |
| Opportunity | opportunity | \- |
| Sales Order | salesorder | \- |

### Related Topics

-   [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3184398.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
