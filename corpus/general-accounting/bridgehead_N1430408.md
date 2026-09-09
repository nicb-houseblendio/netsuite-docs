---
id: "bridgehead_N1430408"
type: "bridgehead"
title: "Classifications and Currency Revaluation"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Foreign Currency Revaluation > Revaluation of Open Currency Balances > Generating Revaluations > Classifications and Currency Revaluation"
parent: "section_N1430227"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1430408.html"
anchors: ["subsect_1556040137", "subsect_1556041020", "svg_2", "svg_2background", "svg_2background_1_", "svg_2Arrows", "svg_2Arrow_1", "svg_2Arrow_1_5_", "svg_2Arrow_1_11_", "svg_2Arrow_1_10_", "svg_2Arrow_1_9_", "svg_2Arrow_1_8_", "svg_2Arrow_1_4_", "svg_2Arrow_1_6_", "svg_2Arrow_1_13_", "svg_2Arrow_1_12_", "svg_2Layer_1", "svg_2Node_4", "svg_2Oval_2_", "svg_2Oval_3_", "svg_2Node_2", "svg_2Node_2_2_", "svg_2Node_2_1_", "svg_2Oval_1_", "svg_2Oval", "svg_2Oval_4_", "svg_2text"]
sha256: "9ca9bff1d2c521c9f06bce072fa4f6a94ec4695bb0d2e5df18df71070ae4dd2a"
---

Classifications are often referred to as segments. Class, department, and location are standard segments. You can also have custom segments that impact the general ledger. For more information, see [Classifications Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261486.html).

The Month End Currency Revaluation page has two areas in which classifications are considered: the classification filters and the Match Source Classifications box.

![Screenshot of Month End Currency Revaluation page with callouts for classification filters and Match Source Classifications box](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/RevalFilters.png)

| **1** | **Classification filters** - In addition to the standard segments shown, each custom segment with GL impact automatically adds a filter. |
| --- | --- |
| **2** | **Match Source Classifications** - This box only affects the revaluation of open receivables and open payables. |

## Classification Filters {#subsect_1556040137}

The filters for standard segments (Class, Department, and Location) behave differently from any custom segment filters. You can use the standard segment filters to limit the accounts list to accounts that are restricted to the classification values you select. Accounts can't be restricted by custom segment, so custom segment filters on this page don't filter the account list.

All selected filter values, including those for custom segments, are copied to the lines in revaluation in the GL Impact subtab. For more information about restricting accounts, see [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html).

If you use the classification filters, you should generate revaluations without filters as a last step before marking the task complete. This last step ensures that you don't accidentally miss accounts that you intended to revalue.

## Match Source Classifications {#subsect_1556041020}

The Match Source Classifications box only affects revaluation of open receivables and open payables. Other accounts are unaffected by this box. This field determines whether classifications are copied to the currency revaluation transactions for open receivables and open payables. The classification values, when copied, appear on the GL Impact subtab of the currency revaluation transaction.

When the Match Source Classification box is checked:

-   If the source transaction has values for **all required** classifications, the classifications from the source transactions are copied to **all** lines in the currency revaluation. One currency revaluation transaction is created for each classification combination.
    
-   If a source transaction **doesn't** include a value for a **required** segment, revaluation fails and you receive an error. Whether standard classifications are required is determined by the accounting preferences Make Departments Mandatory, Make Classes Mandatory, and Make Locations Mandatory. Custom segments also have a Mandatory option.
    
-   If a source transaction is missing a value for a segment that isn't required, any other classification values the transaction has are copied to the currency revaluation. Currency revaluation transactions aren't created for each classification combination.
    

When the Match Source Classification box is clear, classification values aren't copied from the source transactions to the currency revaluation transactions unless a classification filter is applied.

Tip:

To revalue currencies when required segments don't have values, ensure the **Match Source Classification** box is clear.

The following diagram illustrates how classifications are applied to currency revaluations.

<a id="svg_2"></a>

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             

### Related Topics

-   [Generating Revaluations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1430227.html)
-   [Foreign Currency Revaluation for Multiple Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4169300609.html)
-   [Viewing Revaluation Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1430727.html)
-   [Revaluation Record Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1430933.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_2', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_2').resize(); svgPanZoom('#svg\_2').fit(); svgPanZoom('#svg\_2').center(); },false);
