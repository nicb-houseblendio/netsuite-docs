---
id: "section_N2839623"
type: "section"
title: "Setting Sourcing Criteria"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Creating a Custom Field > Setting Sourcing Criteria"
parent: "section_N2829580"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2839623.html"
anchors: ["svg_1", "svg_1Node_23_", "svg_1Node_22_", "svg_1Node_21_", "svg_1Node_16_", "svg_1Node_15_", "svg_1Node_14_", "svg_1Node_8_", "svg_1Node_13_", "svg_1Node_12_", "svg_1Node_11_", "svg_1Node_10_", "svg_1Node_9_", "svg_1Node_7_", "svg_1Node_6_", "svg_1Node_5_", "svg_1Node_4_", "svg_1Node_3_", "svg_1Node_1_", "svg_1Node_20_", "svg_1Node_18_", "svg_1Node_17_", "svg_1Node_19_", "subsect_164321638885"]
sha256: "2d423847d25eda62e901a317a9ea371838fea9d3442ea7d03068b6fd941dd06f"
---

This topic introduces the sourcing and filtering capabilities available for custom fields, including when to store sourced values.

Custom fields can pull values from other records in your account. The information populated in the custom field is then dependent on fields associated with a record selected on another field within that form. Sourcing helps reduce data-entry errors and keeps your forms up-to-date with the latest information your customers and employees need.

You can source data from both standard and custom fields.

For instance, you can have two custom fields, Sales Rep and Sales Rep Email, on a custom case form. When a customer record is selected in the Customer field, the sales representative already defined in the selected customer record is automatically filled in on the Sales Rep field on the case form. The Sales Rep Email field then defaults to the email address defined for the sourced Sales Rep.

The following diagram shows the custom field sourcing and filtering setup required to populate the Sales Rep and Sales Rep Email fields on a custom case form with data from the customer record:

<a id="svg_1"></a>

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           

Note:

The custom field gets updated when the record is created or when specific fields are changed when editing a record. In the preceding example, if you change the sales representative selected on the customer, the sourced field will update to show the new sales representative's email address.

When setting up sourcing, you can choose to store the sourced value in the custom field. If you don't store the value, it's not saved in the custom field. Instead, the field will dynamically pull data from another source stored elsewhere. By not saving the value in the custom field, the field information is instead dynamically populated with data that's stored elsewhere.

You can store a sourced value to prevent it from being overwritten if the source field content changes. To store a value, you need to set up the Source List and Source From fields on the custom field's Sourcing & Filtering subtab. The sourcing automatically fills the custom field with a value when the primary field, defined in the Source List field, is changed. If Store Value is checked, then the value populated in the field is stored on the record. You can optionally change the value on the custom field to have that value stored instead of the populated value. If the value in the source field changes, the stored value won't be overwritten.

For information about how to set up sourcing and filtering criteria, see [Setting Sourcing and Filtering Criteria for a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1024121621.html)

For more information about storing values, see [Setting the Store Value Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1487762215.html).

For information about custom transaction line field sourcing prior to 2021.2, see [Note about Custom Transaction Line Field Sourcing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2839850.html).

## Preserve a Source Value {#subsect_164321638885}

Suppose a custom transaction field sources a sales representative value. When you create sales order SO-123, NetSuite sources John Wolfe, the sales representative for the region.

Later, Mary Brown replaces John as the regional sales representative. Select the Store Value box so that sales order SO-123 continues to show John. The sourced value is retained and is not replaced by Mary.

### Related Topics

-   [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html)
-   [Setting Sourcing and Filtering Criteria for a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1024121621.html)
-   [Custom Fields Sourcing Videos](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1024122002.html)
-   [Note about Custom Transaction Line Field Sourcing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2839850.html)
-   [Troubleshooting Common Sourcing Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0709095341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
