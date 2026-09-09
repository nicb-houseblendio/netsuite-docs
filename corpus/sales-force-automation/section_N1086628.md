---
id: "section_N1086628"
type: "section"
title: "Lead Conversion"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Record Management > Lead Management > Lead Conversion"
parent: "section_N1086131"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1086628.html"
anchors: ["svg_1", "svg_1background", "svg_1Node_15_", "svg_1Node_16_", "svg_1Node_3_", "svg_1Node_17_", "svg_1Node_5_", "svg_1Node_6_", "svg_1Node_8_", "svg_1Node_7_", "svg_1Node_10_", "svg_1Node_9_", "svg_1Node_14_", "svg_1Node_13_", "svg_1Node_12_", "svg_1Node_11_", "svg_1Node_19_", "svg_1Node_18_", "svg_1Node_20_", "svg_1Node_1_", "bridgehead_N1086331", "svg_2", "svg_2Layer_3", "svg_2Layer_1", "svg_2Node", "svg_2Node_00000057856214612517281840000002838153018559781760_"]
sha256: "53146e66d3793877ad72336401dfe128a18ef9555ff3cbbd3679cb8214915821"
---

When a lead qualifies and your sales team is ready to begin entering opportunities and estimates, you are ready to convert the lead to a prospect.

NetSuite has two primary workflows for the conversion of leads. In both workflows, the record workflow is lead to prospect to customer. For a diagram showing a comparison of these workflows, see [Comparing Lead Conversion Workflows](#bridgehead_N1086331).

-   **Conversion by Status Change and Sales Transactions**
    
    In this workflow, lead records are the individuals or companies you're selling to. NetSuite maintains the data on the lead record as it moves up through the sales cycle from lead to prospect to customer. This workflow is often seen in business-to-consumer (B2C) sales organizations.
    
    When a lead is created, it's assigned to a sales representative or team. Whether the assignment is manual or automatic depends on your sales force automation configuration. For information see [Lead Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1093883.html).
    
    Then, the sales representative makes contact with the lead and starts the nurturing process. When negotiations reach the point where a sale seems possible, the representative converts the lead record to a prospect record. The conversion may be a manual change of the Status field on the lead record or an automatic change upon creation of an estimate, opportunity, or sales transaction.
    
    Your administrator configures default statuses for lead, prospect, and customer records on the Sales Preferences page at _Setup > Sales > Preferences > Sales Preferences_. These default statuses control conversion of records from lead to prospect to customer. For information, see [Sales Force Automation Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1035924.html).
    
    For more information about converting leads using this workflow, see [Conversion by Status Changes and Sales Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1086702.html).
    
-   **Conversion with the Lead Conversion Feature**
    
    In this workflow, a lead is an employee or other individual associated with a company you want to sell to. The lead record tracks information about the company you want to sell to. It also tracks information about the individual contact you are speaking with regarding the deal. This workflow is common in a business-to-business (B2B) sales process or in companies with longer sales cycles.
    
    When the lead qualifies, the conversion creates two records: a contact record for the individual and a prospect record for the company. Lead records in this workflow are type individual, but they result in prospects of type company with a linked contact record.
    
    To convert leads in this workflow, click the Convert button on the lead record. You have several options for the records created from the converted lead. For details and instructions, see [Lead Conversion Using the Lead Conversion Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1086741.html).
    
    <a id="svg_1"></a>
    
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         
    

## Comparing Lead Conversion Workflows {#bridgehead_N1086331}

The following illustration shows the records in each of the two lead conversion workflows.

<a id="svg_2"></a>

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   

### Related Topics

-   [Lead Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1086131.html)
-   [Lead Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1086363.html)
-   [Performing a Mass Update on Customer Statuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1087722.html)
-   [Assigning Leads](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1093032.html)
-   [Lead Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1093883.html)
-   [Lead Notification Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1095188.html)
-   [Lead Conversion Reports, Search, and KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1095502.html)
-   [Setting Up Lead Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1093237.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); svgPanZoom('#svg\_2', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); svgPanZoom('#svg\_2').resize(); svgPanZoom('#svg\_2').fit(); svgPanZoom('#svg\_2').center(); },false);
