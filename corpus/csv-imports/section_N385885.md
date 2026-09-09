---
id: "section_N385885"
type: "section"
title: "Projects (Jobs) Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Relationships Import Type > Projects (Jobs) Import"
parent: "section_N383063"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N385885.html"
anchors: ["bridgehead_3796026466", "bridgehead_3796037077", "bridgehead_3796037184", "bridgehead_N386024", "bridgehead_3795977812", "bridgehead_3795903553", "bridgehead_3796037308"]
sha256: "11ef16ebf1ad780c9159d5919d65ed31251d883f8af950a159b664e11e12ba8a"
---

You use the project record to manage company initiatives.

To use the project record, you must have the Projects feature enabled at _Setup > Company > Enable Features_, on the Company subtab. If you plan to do advanced project tracking, you must also enable Project Management. If you don't see the Project Management box, your company must first purchase the Project Management add-on from NetSuite.

To access the project record in the UI, choose _Lists > Relationships > Projects_ (or Jobs). For help working with projects manually, see [Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3714107248.html).

You can import project tasks from a CSV export of Microsoft Project plan data. For more information, see [Project Tasks Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N438898.html).

Note:

As of Version 2008, Release 2, the Jobs feature and the Advanced Job Tracking feature have been renamed to Projects and Project Management, and Job records may be labeled Project records, depending on your account's settings at _Setup > Company > Rename Records/Transactions_.

## Project Body Fields {#bridgehead_3796026466}

This section describes some of the important body fields on the project record.

## Subsidiary {#bridgehead_3796037077}

If your account is using NetSuite OneWorld, the Subsidiary field is required for project imports. CSV file values for subsidiaries should be hierarchical names, in the following format - grandparent : parent : child, for example, Consolidated Parent Company : UK Subsidiary : Euro Subsidiary.

## Customer {#bridgehead_3796037184}

Imported projects can be standalone or associated with an entity such as customer. You may want to use project imports to associate externally maintained project information with NetSuite customer records on an ongoing basis. However, note that you can't use the Import Assistant to update the Customer field on a project record. This restriction is consistent with user interface business rules. If the customer for a project changes, you need to create a new project record rather than update an existing one.

## Project Sublist Fields {#bridgehead_N386024}

The following sublist data is supported for import:

-   Address - Available when Project Management is **disabled**.
    
-   Resource - Available when Project Management is **enabled**.
    

See the following sections for more detail.

## Working with Addresses {#bridgehead_3795977812}

By default, the sublist Address field is read-only, and data from other sublist fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field.

This sublist is selectively updatable based on Internal ID or Label key field.

## Working with Resources {#bridgehead_3795903553}

When using the Import Assistant, the behavior of the Resources sublist differs slightly from the behavior in the UI. Specifically, in the UI, each line must have a unique value in the Name field. Further, in the UI, you can select more than one role for each resource.

![Resource Details subtab.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/ProjectResources_2014_2.png)

With the Import Assistant, if you want to add a resource that has two different roles, you set up your CSV file as if you're adding two sublist records for that resource - one for each role. The Name values aren't required to be unique, as shown in the table below. This example shows how to add two unique resources to the sublist. But because one resource has two roles, the file is set up as if adding three sublist records.

| External Id | CompanyName | Job 1: Name | Job 1: Role | Job 2: Name | Job 2: Role | Job 3: Name | Job 3: Role |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 101A | Launch | John Smith | Installer | John Smith | Designer | Jane Johnson | Staff |

Note that after you complete the add operation, the Resources sublist in the UI looks the same as it would if you had manually added one line for the resource, with multiple roles specified on that line, as shown in the illustration above.

## For More Information {#bridgehead_3796037308}

For details about additional body and sublist fields that can be mapped in the project record, refer to the SOAP Schema Browser's [job](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/job.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Importing Entities and Contacts Together](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N391803.html)
-   [Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3714107248.html)
-   [Creating a Project Resource Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1188929.html)
-   [Understanding Leads, Prospects, and Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N394436.html)

### Related Topics

-   [Relationships Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383063.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
