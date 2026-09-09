---
id: "section_N3366315"
type: "section"
title: "Configuration Bundles"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Types of Bundles > Configuration Bundles"
parent: "section_N3364548"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3366315.html"
anchors: ["bridgehead_N3366368"]
sha256: "8efd03f6d9b84ca5448c485750382f01f4dff18b7feb36e68f6131a852014c02"
---

Configuration bundles let administrators copy setup and configuration settings between accounts. NetSuite vertical solution providers and independent software vendors (ISVs) can use configuration bundles to automate the setup and configuration of a customer account. The supported settings include company preferences, accounting lists, customer relationship management lists, record names, and transaction names. Configuration bundles can also enable or disable features in target accounts.

Note that you cannot include data, such as a chart of accounts, in a configuration bundle. If an object that you install as part of a bundle requires data, then you must import the required data separately from the bundle.

Important:

Install configuration bundles right after provisioning an account. This prevents overwriting existing production account settings. For existing customers, work with account administrators to analyze the impact before installing the bundle if your solution requires specific setup and configuration.

## Objects Available in Configuration Bundles {#bridgehead_N3366368}

The following table lists the types of objects that you can include in a configuration bundle. These objects are preferences and configuration settings. For a description of an object type's function, go to the path shown and see the help for that page.

| Object Type | Object | Navigation Path |
| --- | --- | --- |
| **Auto-Generated Numbers** | Note: Updating a configuration bundle does not change existing auto-generated numbers. |  |
|  | CRM | _Setup > Company > Setup Tasks > Auto-Generated Numbers_ |
|  | Entities | _Setup > Company > Setup Tasks > Auto-Generated Numbers_ |
|  | Schedules | _Setup > Company > Setup Tasks > Auto-Generated Numbers_ |
|  | Transactions | _Setup > Company > Setup Tasks > Auto-Generated Numbers_ |
|  |  |  |
| **Company Preferences** |  |  |
|  | Approval Routing | _Setup > Accounting > Preferences > Accounting Preferences_ |
|  | CSV Import | _Setup > Integration > Manage Integration > SOAP Web Services Preferences_ |
|  | Email | _Setup > Company > Preferences > Printing, Fax & Email Preferences_ |
|  | External | _Setup > Support > Preferences > Support Preferences_ |
|  | Fax | _Setup > Company > Preferences > Printing, Fax & Email Preferences_ |
|  | Forecasts | _Setup > Sales > Preferences > Sales Preferences_ |
|  | General Accounting | _Setup > Accounting > Preferences > Accounting Preferences_ |
|  | General Company Note: Override settings for the preferences on the Overriding Preferences subtab are preserved if the matching preferences are a part of the bundle. | _Setup > Company > Preferences > General Preferences_ |
|  | General Issues | _Setup > Issues > Preferences > Issue Preferences_ |
|  | General SFA | _Setup > Sales > Preferences > Sales Preferences_ |
|  | General Support | _Setup > Support > Preferences > Support Preferences_ |
|  | Inbound Email | _Setup > Marketing > Preferences > Marketing Preferences_ |
|  | Inventory Management | _Setup > Accounting > Preferences > Inventory Management Preferences_ |
|  | Invoicing | _Setup > Accounting > Preferences > Invoicing Preferences_ |
|  | Items / Transactions | _Setup > Accounting > Preferences > Accounting Preferences_ |
|  | Marketing | _Setup > Marketing > Preferences > Marketing Preferences_ |
|  | Notification | _Setup > Accounting > Preferences > Accounting Preferences_ |
|  | Notifications | _Setup > Issues > Issue Preferences_ |
|  | Order Management | _Setup > Accounting > Preferences > Accounting Preferences (Administrator)_ |
|  | Printing | _Setup > Company > Preferences > Printing, Fax & Email Preferences (Administrator)_ |
|  | Shipping | _Setup > Accounting > Setup Tasks > Shipping (Administrator)_ |
|  | Time & Expenses | _Setup > Accounting > Preferences > Accounting Preferences (Administrator)_ |
|  | Web Services | _Setup > Integration > Manage Integrations > SOAP Web Services Preferences(Administrator)_ |
|  |  |  |
| **Features** |  |  |
|  | Company | _Setup > Company > Setup Tasks > Company Information (Administrator)_ |
|  | Accounting | _Setup > Accounting > Preferences > Accounting Preferences (Administrator)_ |
|  | Tax | _Setup > Company > Setup Tasks > Enable Features_ |
|  | Transactions | _Setup > Sales > Preferences > Sales Preferences (Administrator)_ |
|  | Items & Inventory | _Setup > Accounting > Preferences > Accounting Preferences (Administrator)_ |
|  | Employees | _Setup > Users/Roles > User Management > Manage Users (Administrator)_ |
|  | Customer Relationship Management | _Setup > Marketing > Preferences > Marketing Preferences (Administrator)_ |
|  | Web Presence | _Setup > Company > Setup Tasks > Enable Features_ > Web Presence |
|  | SuiteCloud | _Customization > Forms > Transaction Forms (Administrator)_ |
|  |  |  |
| **Other Lists** |  |  |
|  | Accounting Lists | _Setup > Accounting > Setup Tasks > Accounting Lists (Administrator)_ |
|  | Customer Relationship Management (CRM) Lists | _Setup > Sales > Preferences > Sales Preferences (Administrator)_ |
|  |  |  |
| **Renaming** |  |  |
|  | Account Type Names | _Setup > Company > Setup Tasks > Rename Records/ Transactions (Administrator_ |
|  | Record Names | _Setup > Company > Setup Tasks > Rename Records/ Transactions (Administrator)_ |
|  | Transaction Names | _Setup > Company > Setup Tasks > Rename Records/ Transactions (Administrator)_ |

Note:

Inactive settings in the source account are not installed in target accounts when included in a configuration bundle.

Configuration bundles cannot be managed bundles.

### Related Topics

-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Types of Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3364548.html)
-   [Configuration Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3366315.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3364871.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
