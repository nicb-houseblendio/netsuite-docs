---
id: "section_N1263041"
type: "section"
title: "Multiple Shipping Routes"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > Multiple Shipping Routes"
parent: "chapter_N1257369"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263041.html"
anchors: ["procedure_N1263202", "procedure_N1263274", "bridgehead_4565714779", "bridgehead_N1263410", "procedure_N1263424", "bridgehead_N1263509", "procedure_N1263528", "bridgehead_N1263558"]
sha256: "20e5343d549aa430530ab5670033d77fb6796e9150e4c219460518e42cb0ca6c"
---

The Multiple Shipping Routes feature enables you ship to several addresses using different shipping methods on the same transaction.

For example, an order is fulfilled from your Atlanta warehouse. Some items are shipped by FedEx to Mr. Smith in Georgia whereas Mr. Jones receives items in New York through USPS.

The Multiple Shipping Routes feature can be enabled in NetSuite United States edition accounts and NetSuite International edition accounts.

A shipping route is defined as a unique combination of the following:

-   shipping address
    
-   shipping carrier
    
-   shipping method
    
-   origin address
    

If you use SuiteScript or SOAP web services and have enabled Multiple Shipping Routes, see:

-   Multiple Shipping Routes and SuiteScript in [Subrecord Scripting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4675625458.html#subsect_1517631992).
    
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
    
    These sections provide information for developers who work with this feature.
    

Web store shoppers can select multiple shipping addresses for an order during checkout. However only one shipping method can be selected for each shipping address.

To learn more, see [Multiple Ship To](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4188560821.html).

Note:

To charge for shipping see, [Setting Up Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1257579.html).

#### To enable the multiple shipping routes feature: {#procedure_N1263202}

1.  Go to _Setup > Company > Enable Features_.
    
2.  Click the **Transactions** subtab.
    
3.  In the **Shipping & Receiving** section, check the following boxes:
    
    -   **Advanced Shipping** - Provide separate processes to shipping and accounting for fulfilling and billing sales orders
        
    -   **Shipping Label Integration** - Generate tracking numbers and shipping labels when you ship using integrated shipping items
        
    -   **Multiple Shipping Routes** - Ship to multiple destinations using multiple shipping services on a single transaction
        
4.  Click **Save**.
    
5.  If you have a US nexus, perform the following steps:
    
    1.  Go to _Setup > Accounting > Taxes > Set Up Taxes_.
        
    2.  Click the **United States** subtab.
        
    3.  Check the **Per-Line Taxes on Transactions** box.
        
        Only the United States nexus subtab has the **Per-Line Taxes on Transactions** box. Other country nexuses calculate taxes at the line level by default.
        
    4.  Click **Save**.
        
        After you enable Multiple Shipping Routes, the Enable Item Line Shipping box is displayed on standard transaction forms.
        
6.  If the transaction has multiple shipping routes, to enable NetSuite to calculate the correct amounts for each line item, in the transactions **Items** subtab, check the **Enable Item Line Shipping** box.
    
    Each time you create a new customer transaction, check the box to enter multiple shipping routes.
    
    To learn more, see [Adding Multiple Shipping Routes on a Custom Form](#bridgehead_N1263410).
    

To set a default shipping method for an item to ensure that your sales team enters the best shipping method when creating orders.

To learn more, see [Setting a Default Shipping Method Per Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263649.html).

Additional columns are also displayed on the transaction form, so you can select a shipping address for each line item.

#### To add multiple shipping routes on a transaction: {#procedure_N1263274}

1.  From the **Transactions** tab, select a transaction form.
    
    You can use Multiple Shipping Routes on sales orders, estimates, cash sales, product invoices, and credit memos.
    
    To learn more, see the help topic [Working with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N545359.html).
    
2.  On the **Items** subtab, check the **Enable Item Line Shipping** box.
    
3.  In the **Item** column, to select an item click the arrow and then click **List**.
    
4.  Click **Add**.
    
5.  Click the **Shipping** subtab.
    
6.  Select a customer shipping address from the **Ship To Select** field.
    
    To enter a different address, do one of the following:
    
    1.  Select an address from the **Ship To Select** field.
        
        **Legacy Tax**:
        
        When using Legacy Tax, this field displays only addresses in the country of the transaction's nexus.
        
        Examples:
        
        -   If the transaction's nexus is CA-Quebec, all Canadian addresses are available (regardless of whether the subsidiary has other Canadian nexuses).
            
            If the same subsidiary has at least one U.S. nexus, no U.S. addresses are available (regardless of whether the subsidiary has other U.S. nexuses).
            
        -   If the subsidiary has only one U.K. nexus and one German nexus, to create a transaction for a U.K. customer, select a customer address in the U.K. and other countries, except those that are in German in the Ship To field.
            
        
        **SuiteTax**:
        
        When using SuiteTax, this field displays all addresses. You will be able to select different addresses when the nexus determined for the item line is the same as the nexus of the first item line. To learn more, see the help topic [Nexus Determination Lookup Logic in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4283866360.html).
        
        For the following examples, the subsidiary address is in California and has nexuses in U.S-
        
        California, U.S.-New York, and the U.K.
        
        | Transaction Line | Ship From (header location) | Ship To (line level) | Subsidiary has nexus in Ship To State/Country | Nexus determined for the item line | Transaction on Nexus | Result |
        | --- | --- | --- | --- | --- | --- | --- |
        | 1 | California | California | Yes | U.S.-California | U.S.-California | 
        -   The nexus determined for the first item line will be the transaction nexus.
        -   The nexus determined for subsequent item lines will be validated against the transaction nexus.
        -   All item lines must have the same nexus.
        
         |
        | 2 | California | Texas | No | U.S.-California | U.S.-California | Since there is no Texas nexus, the US-California nexus is determined based on the subsidiary's address. |
        | 3 | California | New York | No | U.S.-New York | U.S.-California | 
        
        -   Multiple nexuses on the transaction are not allowed.
        -   You will not be allowed to add the line.
        -   You need to create a separate transaction for this item line.
        
         |
        | 4 | California | Germany | No | U.S.-California | U.S.-California | 
        
        -   There is no Germany nexus, therefore US-California nexus is determined based on the subsidiary's address.
        -   Considered an export transaction.
        
         |
        
    2.  To add a new address saved to the customer record, select **New** or click the **+** (plus) icon.
        
    3.  To enter a custom address, which only stays on the transaction and is not saved to the customer record, select **Custom**.
        
    4.  To edit an existing shipping address, click the edit icon.
        
        To learn more, see the help topic, [Working with Addresses on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N553515.html).
        
7.  Select the address **Ship Method**.
    
8.  To add items to the transaction, repeat Steps 3 - 6.
    
9.  Enter the estimated **Ship Date**.
    
    After fulfillment, the Actual Ship Date field appears on the sales order.
    
    Note:
    
    When working with the feature in SuiteScript or SOAP web services, after the record is submitted NetSuite calculates the shipping group.
    
10.  To ship this order only when complete, check the **Ship Complete** box.
     
     This prevents multiple shipments of part-orders,
     
11.  To generate a list of shipping routes for this transaction, click **Calculate Shipping**.
     
     Whenever the list of transaction items, the Ship To (address), Shipping Method, or Location changes, click Calculate Shipping.
     
12.  Click **Save**.
     

## Shipping and Handling Rules with Multiple Shipping Routes {#bridgehead_4565714779}

After Multiple Shipping Routes is enabled, any shipping or handling rule applied to the transaction is calculated on a line-level basis. For example, when calculating the Free if Total is over rule, the total of items sent to that shipping address determines whether the discount criteria is met, not the value of the combined transactions on the sales order.

To learn more, see [To enable the multiple shipping routes feature:](#procedure_N1263202).

## Adding Multiple Shipping Routes on a Custom Form {#bridgehead_N1263410}

You can use multiple shipping routes even if you use a custom preferred form for entering transactions.

To do this, add the [To add the Enable Item Line Shipping box to a custom form:](#procedure_N1263424) box to the custom form and then [To add multiple shipping routes on a transaction:](#procedure_N1263274) on the transaction.

#### To add the Enable Item Line Shipping box to a custom form: {#procedure_N1263424}

1.  From the **Transactions** tab, select a transaction form.
    
2.  Select your preferred **Custom Form**.
    
3.  In the **Customise** menu, select **Customise Form**.
    
4.  On the **Screen Fields** subtab, click the **Items** tab.
    
5.  Beside **Enable Item Line Shipping**, check the **Show** box.
    
    The **Enable Item Line Shipping** box is displayed in your preferred custom form.
    
    After you check the Enable Item Line Shipping box, the following fields appear:
    
    | Field Name | Description |
    | --- | --- |
    | **Shipping Tax Amount** | Displays the tax amount applied to the shipping rate. |
    | **Handling Tax Amount** | Displays the tax amount applied to the handling rate. |
    | **Shipping Tax Details Reference** | The shipping tax details reference that links the tax line to its corresponding shipping line item. |
    | **Handling Tax Details Reference** | The handling tax details reference that links the tax line to its corresponding handling line item. |
    
6.  Click **Save**.
    
7.  Click the **Transactions** tab to select the transaction form again.
    

## Disabling Multiple Shipping Routes {#bridgehead_N1263509}

NetSuite enables you to turn off the Multiple Shipping Routes feature, even after you have created sales orders with multiple shipping routes. If you disable this feature, all transactions display only one shipping address and shipping method.

Important:

Before turning the feature off, fulfill all outstanding orders with multiple shipping routes.

#### To disable the feature: {#procedure_N1263528}

1.  Go to _Setup > Company > Enable Features_.
    
2.  Click the **Transactions** subtab.
    
3.  In the **Shipping & Receiving** section, clear the **Multiple Shipping Routes** box.
    
4.  Click **Save**.
    

## Return Authorizations with Multiple Shipping Routes {#bridgehead_N1263558}

Return authorizations, or Return Materials Authorizations (RMAs), do not support multiple shipping routes. However, if you bill each fulfillment to a shipping route, you can create RMAs related to an order that uses multiple shipping routes by creating an authorization from those individual cash sales or invoices.

For more information about return materials authorization see, [Return Authorization (RMA) Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1304530.html).

### Related Items

-   [Item Fulfillments and Multiple Shipping Routes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263863.html)
-   [Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1215966.html)
-   [Order Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1222915.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
