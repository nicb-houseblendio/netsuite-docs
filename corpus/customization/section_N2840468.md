---
id: "section_N2840468"
type: "section"
title: "Dependent Dropdown Lists"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Creating a Custom Field > Dependent Dropdown Lists"
parent: "section_N2829580"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2840468.html"
anchors: ["kaltura_player_273"]
sha256: "6ed9db36e0ced32f0ffca7c80495d344c4a87dba3f6c03ba8ae2c987348a07e3"
---

You can create a dependent dropdown list using a List/Record type custom field. Dependent dropdown lists let you filter the choices in a list based on the selections in other fields. For instance, you can add two custom transaction line fields to a transaction form and a third that filters based on selections in the first two.

Watch the following video for an overview of dependent dropdown lists.

<a id="kaltura_player_273"></a>

To understand the content in this topic, you should be familiar with creating custom lists, custom record types, and custom transaction types. For more information, see the following help topics:

-   [Creating a Custom List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852278.html)
    
-   [Creating Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2876492.html)
    
-   [Creating a Custom Transaction Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4172789910.html)
    

To set up field dependencies, you use the Compare To Field column on the Sourcing & Filtering subtab on the custom field page. Use the Compare To Field column to compare values entered in multiple fields on a transaction type or other record type with the values defined on a custom record.

The following screenshot of a Transaction Line Field page for Shirt Style shows the Compare To Field setup.

![Sourcing & Filtering subtab with Compare to Field highlighed.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/MMD_Compare_To_Field.png)

To understand how the feature works, it helps to think in terms of controlling fields versus dependent fields. Controlling fields are used to determine the selections that are available in dependent fields.

For instance, you have a Shirt Style transaction line field that filters based on the selections in the Shirt Color and Shirt Size transaction line fields. Shirt Color and Shirt Size are the controlling fields, and Shirt Style is the dependent field. You create the Shirt Style field on the custom record type.

For an example that illustrates the use of multiple dependent dropdown lists, see [Creating Dependent Dropdown Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162153721460.html).

For a detailed example of creating dependent dropdown lists for a vehicle selection scenario, see [Dependent Dropdown Lists Vehicle Specification Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0923085842.html).

### Related Topics

-   [Dependent Dropdown Lists Videos](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0529034107.html)
-   [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html)
-   [Creating Custom Fields by Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161732113352.html)
-   [Assigning Custom Fields to Specific Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830027.html)
-   [Behavior of View from Order Only Settings on Transaction Line and Transaction Body Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0528113109.html)
-   [Setting Display Options for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830238.html)
-   [Setting Validation and Defaulting Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830711.html)
-   [Setting Sourcing Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2839623.html)
-   [Sourcing and Filtering Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2839994.html)
-   [Setting Filtering Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2840153.html)
-   [Restricting Access to Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2841053.html)
-   [Restricting Access to Employee Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1514478336.html)
-   [Creating Read-Only Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2842596.html)
-   [Adding Translations for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4308565496.html)
-   [Adding Custom Fields to Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828541.html)
-   [Tracking Changes to Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_54095541974.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
