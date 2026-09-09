---
id: "section_N1008542"
type: "section"
title: "Using the Upsell Manager Wizard"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Upsell Manager > Using the Upsell Manager Wizard"
parent: "chapter_N1006631"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1008542.html"
anchors: ["bridgehead_N1008605", "bridgehead_N1008649", "bridgehead_N1008661", "procedure_N1008700", "bridgehead_N1008803", "procedure_N1008838", "bridgehead_N1008968", "procedure_N1008992", "procedure_N1009038", "bridgehead_N1009099", "bridgehead_N1009141"]
sha256: "cdd88619ba85feab2be765502da9d668af4cef19cd7c660be444d85c1051b9c7"
---

The Upsell Manager Wizard walks you through the creation of lists of upsell customers. To upsell with the Upsell Manager, go to _Lists > Marketing > Upsell Manager_.

## Step 1 of 5: Select Upsell Type {#bridgehead_N1008605}

There are two ways to use the Upsell Manager to determine upsell items and target customers. You can base your upsell on:

-   **Items to Upsell** - Select this option to upsell specific items or categories of items.
    
-   **Items Purchased** - Select this option if you do not know which items or item categories you want to upsell. This option lets you search for upsell items based on past purchases.
    

Click **Next**.

## Step 2 of 5: Selecting Upsell Items {#bridgehead_N1008649}

You can either select the items you want to upsell or search for items that provide strong upsell opportunities.

## Upselling Based on Items to Upsell {#bridgehead_N1008661}

To base your upsell on items to upsell, select your upsell items or item categories. You'll see a list of items and categories that have sold well with the upsell items you chose.

Correlation is the percentage of customers who bought both the upsell item and the related item.

Use the selected upsell items to create a list of customers that purchased the correlated item but not the upsell item.

For example, a Wolfe Electronics sales rep wants to upsell service plans. They use Upsell Manager to determine that there is a strong correlation between service plans and laptops. They create a group of customers that purchased laptops but not service plans.

#### To select specific upsell items: {#procedure_N1008700}

1.  Select the items or item categories you want to upsell in the **Items to Upsell** field.
    
    Hold **CTRL** to select more than one item.
    
2.  Set the following upsell search criteria to filter your upsell item search results:
    
    -   **Correlation Greater Than** - NetSuite returns only those items with a correlation greater than what you set in your upsell item search.
        
        Correlation is the percentage of customers that purchased both the upsell items and each item in your upsell search results.
        
    -   **Count Greater Than** - NetSuite returns only those items with a greater count than what you set in your upsell item search.
        
        Count represents the number of customers that purchased both the upsell items and each item in your upsell search results.
        
3.  Click **Search**.
    
    A list of items and categories that have correlation with the upsell items you selected appears.
    
4.  If you need to change your search criteria, make your changes, and click **Refresh**.
    
5.  Check the boxes in the **Apply** column to select the item pairs on which you want to base your upsell.
    
6.  Click **Next**.
    

NetSuite automatically creates a customer search based on items purchased.

You can now set additional criteria for your upsell customer search.

## Upselling Based on Items Purchased {#bridgehead_N1008803}

To base your upsell on items purchased, you first select items customers purchased in the past. Then, NetSuite presents a list of upsell items that sold well with the purchased items.

Correlation is the percentage of customers who bought both the upsell item and the related item.

For example, a Wolfe Electronics sales rep uses Upsell Manager to decide which items they can upsell to their customers. They use Upsell Manager to determine that there is a strong correlation between desktop computers and wireless routers. They create a group of customers that purchased desktop computers but not wireless routers.

#### To select upsell items based on items purchased: {#procedure_N1008838}

1.  Select the purchased items in the **Items to Upsell** field.
    
    Hold **CTRL** to select more than one item.
    
2.  Set the following upsell search criteria to filter your upsell item search results:
    
    -   **Correlation Greater Than** - NetSuite returns only those items with a correlation greater than what you set in your upsell item search.
        
        Correlation is the percentage of customers that purchased both the upsell items and each item in your upsell search results.
        
    -   **Lift Greater Than** - NetSuite returns only those items with a greater lift than what you set in your upsell item search.
        
        Lift is the degree to which the item's correlation exceeds its overall purchase frequency (**correlation - purchase frequency**). Purchase frequency is the percentage of customers who purchased an item.
        
        A high lift implies a more reliable correlation.
        
        For example, Wolfe Electronics sold Dell XPS 13 Developer Edition laptops to 100 customers. Forty of the customers also purchased a premium warranty. The correlation between the laptop and the warranty is 40%. Wolfe has 1000 customers, so the purchase frequency is 10%. The lift is 30%.
        
        Wolfe sold its less expensive Dell Inspiron 15 3000 laptops to 300 customers. 150 of these customers purchased the premium warranty. A correlation of 50% and a purchase frequency of 30%. The lift is 20%.
        
    -   **Count Greater Than** - NetSuite returns only those items with a greater count than what you set in your upsell item search.
        
        Count represents the number of customers that purchased both the upsell items and each item in your upsell search results.
        
3.  Click **Search**.
    
    A list of potential upsell items appears.
    
4.  If you need to change your search criteria, make your changes, and click **Refresh**.
    
5.  Check the boxes in the **Apply** column to select the item pairs on which you want to base your upsell.
    
6.  Click **Next**.
    

You can now set additional criteria for your upsell customer search.

## Step 3 of 5: Additional Customer Criteria {#bridgehead_N1008968}

After you choose your upsell items or item categories, define the list of target customers with the upsell.

By default, the customer search finds customers that purchased the upsell items but not purchased other correlated items. You can set additional criteria if you want to filter the results further.

If you do not want to set additional criteria, click **Next**.

#### To add criteria to the customer search: {#procedure_N1008992}

1.  On the **Criteria** subtab, select a filter.
    
2.  Enter the filter criteria.
    
3.  Click **Add**.
    
4.  Repeat these steps for each additional filter.
    

You can also change the way your customer search results appear.

#### To change how your results display: {#procedure_N1009038}

1.  Click the **Results** subtab.
    
2.  At the top of the subtab, choose which columns determine the order of the list of results.
    
3.  In the **Field** column, select a field to add a column to the results.
    
4.  Click **Add**.
    
5.  Repeat these steps for each new column.
    

After you set additional criteria, click **Next**. NetSuite searches for customers that match your criteria and returns a list of results.

Now, you can preview your list of upsell customers.

## Step 4 of 5: Previewing Your Upsell Customer List {#bridgehead_N1009099}

To exclude customers from the upsell effort, clear the box in the **Apply** column next to the customer's name.

To return to the search criteria page, click **Back**. To accept the customer list, click **Next**.

Note:

When you click **Next** NetSuite does not contact customers.

After you choose the customers you want to include, you can choose upsell actions.

## Step 5 of 5: Choosing Upsell Actions {#bridgehead_N1009141}

The Choose Upsell Action page provides four actions for how NetSuite should proceed with this upsell effort. You can choose any of these actions.

For each upsell action, enter information in the fields provided. NetSuite uses this information when it creates records.

For example, a Wolfe Electronics sales rep chooses to create opportunities from upsell customer search results. In the Title field, they enter **Store Warranty Upsell**. For the expected close date, they enter the last day of the month. NetSuite creates an opportunity for each customer in the upsell customer results list with the same title and expected close date.

-   **Create a group of customers to upsell to**
    
    If you choose this action, NetSuite creates a group record from this list of upsell customers. You can then create a marketing campaign targeting this group or perform a bulk merge that offers the upsell items to these customers.
    
-   **Create tasks for the sales reps assigned to the upsell customers**
    
    If you choose this action, NetSuite creates task records for the sales rep assigned to each customer.
    
-   **Schedule phone calls for each upsell customer**
    
    If you choose this action, NetSuite creates phone call records for the sales rep assigned to each customer.
    
-   **Create opportunities for each upsell customer**
    
    If you choose this action, NetSuite creates opportunity records for each customer. These opportunities have the upsell items selected, by default.
    

Note:

You can create opportunities only for upsell items. You can't add item categories to opportunities.

After you choose your upsell actions, click **Finish**.

### Related Topics

-   [Upselling From Customer Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1009337.html)
-   [Upselling on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1009585.html)
-   [Upsell Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1009768.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
