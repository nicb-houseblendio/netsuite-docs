---
id: "section_N1764883"
type: "section"
title: "Frequently Asked Questions about Gross Profit"
branch: "order-management-reports"
category: "order-management"
breadcrumb: "Order Management > Order Management Reports > Estimating Gross Profit > Frequently Asked Questions about Gross Profit"
parent: "chapter_N1752442"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1764883.html"
anchors: ["question_N1764903", "question_N1764933", "question_N1764972", "question_N1765003", "question_N1765045", "question_N1765075", "question_N1765112", "question_N1765142", "question_N1765180", "question_N1765239", "question_N1765269", "question_N1765299", "question_N1765321", "question_N1765347", "question_N1765372", "question_N1765406", "question_N1765467", "question_N1765489", "question_N1765515", "question_N1765544"]
sha256: "d21c6c9dd4170801d6145bb6ab2c00302c8a2cedd539ac1f0e8a4b2763a12220"
---

### What does each of the Gross Profit related fields mean? {#question_N1764903}

See [Using Gross Profit Fields on Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1762276.html).

### My administrator enabled the feature, but I don't see any of the fields you mentioned? {#question_N1764933}

The gross profit fields are automatically added to standard transaction forms when the feature is enabled, but custom forms must be manually changed to include the fields. For more information, see [Enabling the Gross Profit Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1756926.html) and [Using Gross Profit Fields on Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1762276.html).

### I don't see any new gross profit reports. How do I get at this information? {#question_N1764972}

There are no new reports created specifically for gross profit, but you can add the gross profit fields to most sales reports. The fields are also available for advanced and saved searches of transactions. For more information, see [Including Gross Profit Values in Reports, Searches, and KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1763752.html).

### Can I base commissions or track quotas on gross profit? {#question_N1765003}

You can base commission and quotas on gross profit by using the Alternate Sales Amounts (ASA) feature. For information, see [Commission on Estimated Gross Profit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1146536.html).

To do this, you must use SuiteScript to copy the value in the Gross Profit field to the Alt. Sales field. You then create Alt. Sales quotas and commission reps based on those values. For more information, please contact your NetSuite account representative. See [Gross Profit Fields in SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1764294.html#bridgehead_N1764562).

### How does this new gross profit interact with preexisting gross profit functionality, such as the item profitability report? {#question_N1765045}

The costing information currently tracked by the system is the same information that is used by the Gross Profit feature. For example, if average cost is tracked on inventory items, then by setting the Cost Estimate Type to Average Cost (see [Working with Cost Estimate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757575.html)), the average cost for that item will be used in the gross profit calculation on an order. There is otherwise limited interaction between other profit functions, such as item profitability reporting, and the Gross Profit feature.

### Can I prevent some users from seeing the gross profit fields? {#question_N1765075}

Gross profit fields display by default on standard transaction forms after the Gross Profit feature has been enabled. You can hide the gross profit fields from transactions using form customization. For more information, see [Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2852749.html).

### Which transactions have the gross profit fields? {#question_N1765112}

When the Gross Profit feature is enabled, the following standard transaction forms display gross profit fields: Cash Refund, Cash Sale, Credit Memo, Estimate, Invoice, Opportunity, Return Authorization, and Sales Order. For more information, see [Using Gross Profit Fields on Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1762276.html).

### How can I control the use of the Gross Profit feature? {#question_N1765142}

A permission (see [Granting the Override Estimated Costs on Transactions Permission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757391.html)) and a preference (see [Setting the Recalculate Estimated Cost on Creation of Linked Transactions Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757197.html)) can be used to control the feature. Users cannot edit the cost estimate type on transactions, unless they are assigned the permission. The automatic updating of estimated cost information through the sales cycle depends on the setting for the preference.

### How does the feature interact with other features? {#question_N1765180}

The Gross Profit feature is not directly dependent on other features, but may have limited utility without them. For example, if you do not have the Inventory feature enabled, you would not be able to access some costing fields on item records. Following is a list of related, but not dependent features:

**Inventory** - required for certain item types and costing information

**Sales Orders, Opportunities, Estimates** - these features are required to get gross profit information on those transaction types

**Advanced Jobs** - required to get job costing information on sales transactions

**Drop Shipments & Special Orders, Purchase Orders** - required for the Purchase Order Rate Cost Estimate Type to be used. For more information, see [Cost Estimate Type Descriptions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757784.html).

### What is a cost estimate type? {#question_N1765239}

A cost estimate type is a definition of how costs should be estimated for an item; these estimated costs are used to calculate estimated gross profit for the item. A default cost estimate type is defined on the Inventory subtab of item records, users with permission can change the cost estimate type per line item on transaction forms. See [Working with Cost Estimate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757575.html).

### Why is the cost estimate type defined on both the item and the transaction? {#question_N1765269}

The cost estimate type on the item record allows the setting of a default cost estimate type that is set when that item is added to transactions. A user with the appropriate permission (see [Granting the Override Estimated Costs on Transactions Permission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757391.html)) can change the cost estimate type on the transaction after the type has been defaulted in from the item.

### If the Revenue Recognition feature is enabled, are rev rec settings factored into gross profit calculations? {#question_N1765299}

No. Gross profit calculations use the amount and cost of each transaction line, factoring in line-level and transaction-level discounts. Neither cost nor revenue are amortized.

### Are landed costs factored into the gross profit values? {#question_N1765321}

No, gross profit calculations only consider **estimated** costs. Landed costs are excluded from these calculations.

### Can I get the actual costs or only the estimated costs and margin? {#question_N1765347}

Only the estimated costs and margin. Gross profit calculations only consider **estimated** costs, not actual costs.

### Let's say I'm using the Purchase Order Rate for the cost estimate type on an item. After the actual cost is known, could I update the purchase order and have the system then update all related transactions? {#question_N1765372}

No, changes to the purchase order rate would only be reflected in related transactions during the creation of **linked** transactions, and then only if the preference for automatic update is set. See [Setting the Recalculate Estimated Cost on Creation of Linked Transactions Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757197.html).

### My company uses the Project Management feature. How does the costing information from the job get factored into gross profit? {#question_N1765406}

If you add a project to a transaction line, the cost from the related service item will be used. However, if you create the order (or source in) the project to the sales order, then the sum of the estimated costs on the related project tasks will be used. The cost estimate type in this case will be set to **Custom**.

### What happens when I disable gross profit? {#question_N1765467}

All of the related fields will be removed from forms, reports, and searches. SOAP web services integrations and SuiteScripts that are dependent on those fields will fail.

### Why do all of my historical transactions have no gross profit? {#question_N1765489}

Gross profit information is only available on transactions created **after** the feature is enabled.

### Are the gross profit fields available in SuiteScript? {#question_N1765515}

Yes. If the SuiteScript runs with sufficient permission, you can change the values as needed. See [Gross Profit Fields in SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1764294.html#bridgehead_N1764562)

### Are the cost fields available in SOAP Web Services and CSV? {#question_N1765544}

Yes. See [Using Gross Profit Values in CSV Import, SOAP Web Services, and SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1764294.html).

### Related Topics

-   [Estimating Gross Profit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1752442.html)
-   [What is Gross Profit?](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1752846.html)
-   [Who Uses Gross Profit and Why?](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1753013.html)
-   [Setting Up Gross Profit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1756747.html)
-   [Working with Cost Estimate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757575.html)
-   [Using Gross Profit Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1762134.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
