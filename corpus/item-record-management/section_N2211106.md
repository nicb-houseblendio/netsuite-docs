---
id: "section_N2211106"
type: "section"
title: "Standard Costing FAQ"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Standard Costing > Standard Costing FAQ"
parent: "section_N2199708"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211106.html"
anchors: ["question_4417990386", "question_N2211141", "question_N2211167", "question_N2211189", "question_N2211210", "question_N2211239"]
sha256: "7a0ea4cca4a68d0208dc42fd455caaaec74f343a76867ea2b826e23a01a2adec"
---

### Is the Standard Cost field available to update using Mass Updates? {#question_4417990386}

No. The **Standard Cost** field is available in CSV Import and SOAP web services only.

### Can the Inventory Cost Revaluation transaction be backdated? {#question_N2211141}

Yes, if the transaction isn't dated in a closed accounting period.

### Will the automated planned standard cost include components that use the Average costing method? {#question_N2211167}

Yes. The item doesn't have to use the Standard costing method to be selected for the cost rollup.

### Is the Standard Cost field available on an assembly item record? {#question_N2211189}

No. The **Standard Cost** field isn't available on assembly item records because it's generated through the cost rollup.

### Is it possible to create multiple revaluations per location for an item in one day? {#question_N2211210}

No. There can only be one inventory revaluation for an item per day for each location. If you do this, you'll see this message: 'An inventory cost revaluation already exists for this item, location, and date.'

Note:

If you choose to manually add a revaluation, delete the existing revaluation, or change the transaction date. If you run the revaluation on a date that already has one, the existing one updates with new values.

### If I change the Standard Cost value on the item record, will the item's planned standard cost automatically update and be revalued? {#question_N2211239}

No, it's not automatic. You can choose to do one of the following:

-   Edit the planned standard cost record of the item manually and then run a revaluation.
    
-   Process another cost rollup and then run a revaluation.
    

### Related Topics

-   [Standard Costing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705144712.html)
-   [Standard Costing Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162705257513.html)
-   [Enabling Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2200714.html)
-   [Creating Cost Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201059.html)
-   [Creating Inventory Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159673804330.html)
-   [Setting Up Item Records for Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2201836.html)
-   [Defining Cost Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2202327.html)
-   [Entering Planned Standard Cost Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2202799.html)
-   [Standard Cost Rollup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2204939.html)
-   [Revalue Standard Cost Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2205401.html)
-   [Standard Costing and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2206397.html)
-   [Assembly Build Production Cost Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2209083.html)
-   [Standard Costing Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2211461.html)
-   [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
