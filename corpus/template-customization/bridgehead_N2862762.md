---
id: "bridgehead_N2862762"
type: "bridgehead"
title: "Using Advanced Template Formatting Programmatically"
branch: "template-customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Template Customization > Advanced PDF/HTML Templates > Using Advanced Template Formatting Programmatically"
parent: "chapter_4453550706"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2862762.html"
anchors: []
sha256: "4d0b52148b7d05031f0ac5372e5518fc86350239c0e9d8354e1740702590e179"
---

Important:

SuiteScript doesn't support direct access to the NetSuite UI through the Document Object Model (DOM). You should access the NetSuite UI only by using SuiteScript APIs. For information about using SuiteScript APIs to customize the UI, see [SuiteScript 2.1 Custom Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1518456405.html).

SuiteScript supports a template engine object and related methods so you can apply advanced template format capabilities programmatically. For SuiteScript 2.0, see [render.TemplateRenderer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4412065265.html).

In addition, the SuiteScript functions [render.bom(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_457552429198.html) [render.packingSlip(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_458625732421.html) [render.pickingTicket(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_456921936034.html) [render.statement(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_455095458983.html) [render.transaction(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_452452331542.html) support the use of advanced templates. If you associate an advanced template with the custom form saved for a transaction and use this API to print the transaction, the advanced template is used to format the printed transaction.

You can use SuiteScript to apply advanced templates to printed records that aren't transactions. See [Using SuiteScript to Apply Advanced Templates to Non-Transaction Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4259402776.html).

### Related Topics

-   [Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453550706.html)
-   [Account-Specific Domains in Advanced Printing Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_159560197793.html)
-   [Enabling the Advanced PDF/HTML Templates Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2862977.html)
-   [Reviewing Available Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2863143.html)
-   [Advanced PDF/HTML Multi-Currency Statement Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4364689607.html)
-   [Setting Custom Forms to Use Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2863334.html)
-   [Advanced Templates Customization in the Template Editor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2863632.html)
-   [Scripting with Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1533138530.html)
-   [Changing the Script ID of a Custom Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515580300.html)
-   [Advanced Templates for Printing Saved Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4823423235.html)
-   [Advanced Templates Support for Company Printing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3950986508.html)
-   [FAQs for Advanced Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159984373188.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
