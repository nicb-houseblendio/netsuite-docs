---
id: "section_N1069843"
type: "section"
title: "Preparing an Estimate"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Opportunities and Estimates > Estimates > Preparing an Estimate"
parent: "section_N1069662"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1069843.html"
anchors: ["procedure_N1069882", "procedure_N1072488", "procedure_N1072690", "procedure_N1072752", "procedure_N1072784", "procedure_N1072939", "procedure_N1072996", "procedure_N1073117"]
sha256: "8b2451ed3f1005dd99ae9e19214cea44e52f856edebaee13774f44524af46583"
---

To enable the Estimates feature, an administrator can go to _Setup > Company > Enable Features_. On the **Transactions** subtab under Basic Features, check the **Estimates** box, and then click **Save**.

Note:

Estimates are non-posting transactions.

#### To prepare an estimate: {#procedure_N1069882}

1.  Go to _Opportunities > Transactions > Estimates > New_.
    
2.  Under Primary Information:
    
    1.  In the **Custom Form** field, accept the **Standard Estimate** form or select an existing custom form.
        
        You can also click **New** to customize an estimate form.
        
    2.  Accept or enter the estimate number in the **Estimate #** field.
        
    3.  In the **Customer:Job** or **Project** field, select a customer or project.
        
        If you don't use the **Auto Fill** preference, click **Auto Fill** to fill information from the last transaction for this customer or project.
        
    4.  Enter a title for this estimate. The estimate title text appears on lists, in search and reporting results, and on the **Estimates** subtab of records with which it is associated.
        
        When an estimate is converted from an opportunity, the title from the opportunity defaults into the title field on the estimate. If there is already an estimate against the opportunity, the second estimate has a number following the title.
        
        For example, if the first estimate title is **Project Estimate**, the second estimate title will be **Project Estimate1**. For each subsequent estimate created against that opportunity, the number in the title increases by 1. This distinguishes multiple estimates associated with a single opportunity.
        
        The estimate title field is also available for customization, inline edits, and mass updates.
        
    5.  Enter the date this estimate expires.
        
    6.  Accept or enter the date in the **Date** field.
        
    7.  In the **Status** field, select a status for this estimate.
        
    8.  In the **Probability** field, enter a probability for this estimate.
        
        If you use weighted forecasts, your forecast report only shows the estimate total multiplied by the probability percentage.
        
    9.  Enter the expected close date for this estimate.
        
    10.  When enabled, select a **Sales Channel**.
         
         To learn more, see [Enabling Sales Channels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161348620247.html) Enabling Sales Channels.
         
    11.  Optionally, enter a memo.
         
3.  Under Sales Information:
    
    1.  In the **Opportunity** field, select the opportunity for this estimate.
        
    2.  To include this estimate in your sales forecast, check the **Include In Forecast** box. It appears only if the probability exceeds the minimum forecast probability set by an administrator at _Setup > Sales > Preferences > Sales Preferences_.
        
        If you use the **Advanced Forecasting** feature, select the forecast category this estimate belongs in.
        
    3.  Select the lead source you want to associate with this estimate.
        
    4.  The partner associated with this customer or prospect appears in the **Partner** field. You can choose a different partner for this opportunity.
        
        If you use the **Multi-Partner Management** feature, you can associate partners with this transaction on the **Partners** subtab. For more information, see [Associating Partners With Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167413.html).
        
4.  Under Classification:
    
    Note:
    
    If you use NetSuite OneWorld and the selected customer is shared with multiple subsidiaries, you can choose any subsidiary assigned to the selected customer. For information about sharing customer records with multiple subsidiaries, see [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
    
    1.  If you track departments, select a department.
        
    2.  If you track classes, select a class.
        
    3.  If you track locations, select a location.
        

#### Items {#procedure_N1072488}

1.  If a promotion code applies to this estimate, select it in the **Promotion Code** field.
    
2.  If a transaction discount applies to this estimate, select it in the **Transaction Discount** field.
    
3.  In the **Rate** field, enter any other discounts you want applied to this estimate.
    
    To subtract a discount from your total, enter a negative amount or percentage.
    
    For example, if you want to offer a discount of ten percent, enter -10%.
    
4.  Click **Add Multiple** to add multiple line items at one time.
    
    Click **Upsell Items** to select items for this customer.
    
    Click **Clear All Lines** to remove the line items from the **Items** subtab.
    
5.  In the **Item** column, select an item.
    
6.  In the **Quantity** column, enter the quantity for this item.
    
    The quantity you enter must not exceed 200,000.
    
7.  If you use multiple prices, in the **Price Level** column, choose a price level for this item.
    
    If you choose **Custom**, you can enter a custom price for this item in the **Unit Price** column.
    
    This price applies to this transaction only.
    
8.  If this item is taxable, check the **Tax** box.
    
9.  Check the **Exclude Item from Rate Request** box if you want to exclude the item when calculating shipping. The shipping rate total will not include this item. This box is available only for inventory and assembly items.
    
10.  Set any options that apply to this item.
     
     NetSuite automatically calculates the sales amount and alternate sales amount (ASA). The **ASA** column appears only if you use the **Alternate Sales Amount** feature. For more information, read [Alternate Sales Amounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1049780.html).
     
11.  Click **Add** to add the item to the estimate.
     
12.  Repeat the steps above for each item in this estimate.
     

#### Shipping {#procedure_N1072690}

1.  In the **Shipping Carrier** field, select a carrier.
    
2.  In the **Ship Method** field, choose a shipping method.
    
3.  The shipping total is calculated in the **Shipping Cost** field. Click the **Calculate** icon to reset the cost after you edit the order.
    
    The **Handling Cost** field displays the handling fee associated with the shipping item selected or the items ordered.
    

#### Billing {#procedure_N1072752}

1.  Select the billing address for this estimate.
    
2.  Click **New** to enter a new address.
    

#### Accounting {#procedure_N1072784}

1.  If you use the **Multiple Currencies** feature, the current exchange rate for this customer's currency appears in the **Exchange Rate** field.
    
    You can change the exchange rate for this transaction only, or you can update the currency record with the new exchange rate.
    
    The customer's currency appears in the **Currency** field. All currency amounts on this transaction are shown in this currency.
    
2.  If you use the **Multiple Currencies** feature, select the currency you want to use for this transaction. Only the currencies set on the customer's record are available in this field. The customer's primary currency appears by default. For more information, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).
    
    If you change the currency on the record, NetSuite updates prices and amounts to the currency you select.
    
3.  If you want to charge sales tax on this estimate, check the **Taxable** box.
    
4.  In the **Tax** field, choose the tax rate for this customer.
    
5.  Accept or enter the tax rate in the **Tax %** field.
    

#### Relationships {#procedure_N1072939}

1.  To add a contact to this estimate, enter the contact's name in the **Contact** column.
    
2.  Enter the email address, phone number, job title, and contact's role.
    
3.  Click **Add**.
    
4.  Repeat these steps for each contact you want to attach.
    

#### Sales Team {#procedure_N1072996}

1.  Associate sales reps with this transaction in one of the following ways:
    
    -   If you do not use the **Team Selling** feature, select the sales rep or sales group in the **Sales Rep** field.
        
        The sales rep or sales group associated with the customer on this transaction appears by default.
        
    -   If you use the **Team Selling** feature, click the **Sales Team** subtab.
        
        Select the sales team for this transaction. For more information, see [Associating Partners With Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167413.html).
        
2.  You can change a team member's sales role or contribution for this transaction. Click the employee's name to edit the line.
    
3.  To add an employee to this team for this transaction, click an empty line. Select the employee, set a sales role and contribution, and then click **Add**.
    

#### Communication {#procedure_N1073117}

1.  On the **Messages** subtab, check one or more of these three boxes:
    
    -   Check the **To Be Printed** box if you want to save the estimate form in a queue for printing later.
        
    -   Check the **To Be Emailed** box and then enter or verify an email address if you want to email the estimate form.
        
    -   Check the **To Be Faxed** box and then enter or verify a fax number if you want to fax the estimate form.
        
        Alternatively, you can click **Print** after you enter all of the information to immediately save and print the estimate.
        
2.  Check the **Available in Customer Center** box to share the estimate with your customer through the customer center. Clear the box to save the estimate without making it available in the customer center.
    
3.  Select a customer message to appear on your estimate.
    
    Administrators can create new customer messages at _Setup > Accounting > Setup Tasks > Accounting Lists > New_.
    
4.  Create any events, tasks, or phone calls you want to associate with this estimate.
    
5.  On the **Files** subtab, attach any files you want to associate with this estimate.
    
6.  On the **User Notes** subtab, enter any internal notes related to this estimate.
    
7.  Click **Save**.
    

### Related Topics

-   [Estimates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1069662.html)
-   [Converting an Estimate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1073352.html)
-   [Printing an Estimate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1073538.html)
-   [Deleting Old Estimates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4453306500.html)
-   [Estimates Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1073899.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
