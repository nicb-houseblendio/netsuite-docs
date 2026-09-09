---
id: "section_N1742630"
type: "section"
title: "Understanding EITF 08-01 Revenue Recognition"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > EITF 08-01 Revenue Recognition Feature > Understanding EITF 08-01 Revenue Recognition"
parent: "chapter_N1742394"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1742630.html"
anchors: ["bridgehead_N1742970", "bridgehead_N1743043", "bridgehead_N1743064"]
sha256: "5ee920ae2312454767a40c82e68e68c8d505ca2c02fb4e1d115eda49457be13d"
---

Important:

EITF 08-01 Revenue Recognition is a managed SuiteApp (Bundle ID: 29321).

EITF 08-01 Revenue Recognition stores multiple estimated selling prices (ESP) for each product or service you sell. It tracks an item price, and optionally, an upper and lower price range limit, for each combination of selling dimensions you identify. By default, the price range limit for an ESP is 0. Price range limits are percent based and can be changed over time.

Using formulas linked to the categories of items being sold, EITF 08-01 Revenue Recognition allocates the ESP amount to transaction lines per dimension combination on sales transactions.

For example, a company tracks sales by currency for EITF 08-01 reporting purposes. The Multiple Allocation Prices list stores an estimated selling price for each item for each sales dimension combination as shown below.

![Screenshot of Multiple Allocation Price List showing estimated selling price for each item for each sales dimension combination](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/RevenueExpenseRecognition/eitfpricelist.png)

On sales orders, the following fields identify whether items on the order require pricing allocation for EITF 08-01 Revenue Recognition. You can set the default values for these fields during implementation. Pricing allocations are shown in the VSOE field for a transaction line.

-   **Transaction Is VSOE Bundle** - indicates if the transaction items on the order are related and bundled together for advanced revenue recognition purposes.
    
-   **Auto Calculate VSOE Allocation** - indicates whether to calculate the allocation amount for items automatically when you save the sales order.
    
-   **Transaction Is E81 Bundle** - indicates if revenue recognition for the transaction items on the order is allocated using estimated selling prices according to EITF 08-01 rules. This box must be checked to calculate EITF 08-01 allocations.
    
    Important:
    
    When a sales order or return authorization is enabled with revenue commitment, by default the EITF 08-01 rules for allocating revenue don't apply to sales invoices created from the sales order, or to credit memos from the return authorization. This means that the **Transaction is E81Bundle** preference on the invoice and credit memo transactions is turned off by default. You can apply this restriction to cash sales created from a sales order, and to cash refunds created from a return authorization, by manually deploying the appropriate EITF 08-01 scripts to the transaction forms. For the instructions, see [Applying EITF 08-01 Scripts to Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0806035426.html).
    
    For more information about EITF 08-01 script deployment, see [EITF 08-01 Script Deployment](#bridgehead_N1743064).
    

The EITF-08-01 functionality requires the NetSuite VSOE feature as a prerequisite. If you check the **Transaction is E81 Bundle** box on a sales order, the **Transaction is VSOE Bundle** box is also checked. If you clear the **Transaction is VSOE Bundle** box, the **Transaction is E81 Bundle** box is also cleared.

When you check **Transaction is E81 Bundle**, the **Auto Calculate VSOE Allocation** box is also checked. For transactions that comply only with VSOE requirements, Auto Calculate VSOE Allocation can be checked or cleared.

Price allocations for EITF 08-01 transactions can be calculated automatically or on demand as determined by the **Auto Calculate Revenue Allocation** preference. With the preference enabled, NetSuite calculates allocations for the VSOE field for transaction lines automatically when you edit a transaction. By default, this preference is checked. To improve performance, clear the **Auto Calculate Revenue Allocation** preference box. When you clear the preference, the **Auto Calculate VSOE Allocation** box on the sales order is also cleared. You can then use the **Allocate Multi-element Sales Revenue** button on the sales order to allocate revenue when needed.

Note:

If you clear the **Auto Calculate Revenue Allocation** preference, you can manually check the **Auto Calculate VSOE Allocation** box on sales orders.

Transaction lines on orders that must comply with EITF 08-01 reporting rules to display the estimated selling price allocation information in the VSOE Allocation field group, shown below.

![Screenshot of VSOE Allocation field group](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/RevenueExpenseRecognition/eitfvsoeesp.png)

-   **Allocation Type** - default for this field is Normal
    
    -   **Normal** - revenue recognition for the item follows EITF 08-01 rules.
        
    -   **Exclude** - indicates the item is exempt from revenue allocation and the item selling price is used for revenue recognition.
        
    -   **Software** - the item is software and both EITF 08-01 and SOP 97-2 revenue recognition rules apply for allocating revenue.
        
        Note:
        
        Don't set **Allocation Type** to **Software** if you use the VSOE feature without the EITF bundle.
        
-   **Estimate** - indicates that the item price is the estimated selling price from the Multiple Allocation Price List and the IsVSOE box is clear for the item. This value for this field defaults from the item record.
    
-   **Allocation Price** - the estimated selling price for the item, referenced from the Multiple Allocation Prices list
    
-   **Calculated Amount** - total estimated selling price (ESP) amount for the transaction line calculated using a pre-defined formula (for example, price x quantity) when you save the order
    
-   **Allocation Amount** - revenue amount allocated to transaction line for revenue recognition purposes, based on item category formula and calculated when you save the order
    

## Formulas {#bridgehead_N1742970}

EITF 08-01 Revenue Recognition calculates price allocations according to a formula associated with the item category of the product or service on the transaction line. When you set up EITF 08-01 Revenue Recognition, the following formulas are available:

-   License - Perpetual
    
-   License - Term
    
-   Maintenance/Support
    
-   Services
    
-   Training
    
-   Hardware
    
-   Other
    

EITF 08-01 Revenue Recognition uses the estimated selling price data and the sales dimensions you specify. When you enter sales that must be reported on your books following the EITF 08-01 accounting rules, the estimated selling price amount for each transaction line is allocated using the formula associated with the item category and revenue recognition schedules associated with the transaction line.

Add a saved search and portlet to your dashboard to view multiple allocation price information. Allocated price information is presented in real-time.

## EITF 08-01 and VSOE Reporting Rules {#bridgehead_N1743043}

With EITF 08-01 Revenue Recognition, you can apply both Emerging Issues Task Force Rule 08-01 (EITF) and Statement of Position No. 97-2 (VSOE) revenue recognition rules to items bundled on a single sales order. See [Two-Step Revenue Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1744063.html).

## EITF 08-01 Script Deployment {#bridgehead_N1743064}

The EITF 08-01 scripts are deployed to the following transaction types :

-   Sales Order
    
-   Invoice
    
-   Return Authorization
    
-   Credit Memo
    

This means that the EITF 08-01 rules for allocating revenue apply to these transaction types. On a return authorization, for example, allocation amounts aren't sourced or carried over from a linked invoice and are instead recalculated automatically. Revenue allocation for partial returns are recalculated and only if processing a 100% return do the source invoice and return authorization show the same allocation amount.

On the other hand, by default the EITF 08-01 scripts aren't deployed to Cash Sale and Cash Refund transactions. This means that the EITF 08-01 logic doesn't apply to transactions of these types. For example, on a cash sale created from a sales order that has revenue commitment enabled, the **Transaction is E81 Bundle** preference remains enabled. This is the same behavior on a cash refund created from a return authorization. On invoice and credit memo forms, to which the EITF 08-01 scripts apply, the **Transaction is E81 Bundle** box is turned off by default when the originating transactions (sales order and return authorization, respectively) have revenue commitment enabled.

Note:

Revenue commitment is enabled on a transaction when the Rev Rec on Rev Commit. box is checked.

If you want the EITF 08-01 logic to apply to cash sales and cash refunds, you must manually deploy the scripts to the transaction forms. For the steps, see [Applying EITF 08-01 Scripts to Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0806035426.html).

Note:

If you no longer use the EITF 08-01 scripts and you want to disable them, you should clear the **Deployed** box on the script deployment record to undeploy the script, instead of checking the **Inactive** box on the script record to inactivate it. When SuiteApps are updated, all script records are restored, but script deployments are preserved.

You can view the script deployment records at Customization > Scripting > Script Deployments.

### Related Topics

-   [EITF 08-01 Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1742394.html)
-   [Understanding EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1742630.html)
-   [Contingent Revenue Handling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1743516.html)
-   [About Installing EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746114.html)
-   [Implementing EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746357.html)
-   [Applying EITF 08-01 Scripts to Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0806035426.html)
-   [Working with Estimated Selling Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1747534.html)
-   [How Can I Get This Feature?](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1749904.html)
-   [Revenue and Expense Recognition Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1675871.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
