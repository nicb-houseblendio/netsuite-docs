---
id: "section_N1302167"
type: "section"
title: "Sending Collection Letters in Bulk"
branch: "overdue-balances-and-collections"
category: "order-management"
breadcrumb: "Order Management > Overdue Balances and Collections > Collections > Sending Collection Letters in Bulk"
parent: "chapter_4418080075"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1302167.html"
anchors: ["procedure_N1302182"]
sha256: "a14e692340cfe5732fa207fdbc96f164541d2b01e312b1383135bc9b53a7c8ec"
---

To manage collections, set up a group based on a search for customers with balances past due for 30,60 or 90 days. You can then use the Mail Merge feature to generate a notice to send to customers via e-mail, letter or fax.

For example, customer Mary Smith's last statement showed a balance of $100.00, due on March 15. On April 30, you create a group of customers with overdue balances over 30 days, and she is included in the search results. Using the Mail Merge feature, you can send a bulk e-mail merge to customers included in your search results. Mary then receives a personalized e-mail notifying her of the overdue balance.

#### To send collection notices in bulk: {#procedure_N1302182}

1.  Create a group with a new search for customers with overdue balances at _Lists > Relationships > Groups > New_.
    
2.  On the Create Group page, select **Dynamic** and include customers in the dropdown.
    
3.  Create a name for this group, such as Customers Overdue 30 Days.
    
4.  In the **Saved Search** field, select **New** to create a new search to define this group.
    
    You can use the following filters and criteria:
    
    -   Overdue Balance: Is greater than 0
        
    -   Transaction Fields: Days Overdue: Is greater than or equal to 30
        
    -   Global Subscription Status: Any of **Confirmed Opt-In** and **Soft Opt-In**.
        
    
    For more information on saving searches, see [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html).
    
5.  Click **Save**.
    
    Your search is now saved, and the Customer Group page opens so that you can complete your group.
    
6.  Click **Save**.
    
7.  Create a template for your collections notice.
    
    You can create your template externally and upload the template from the template record or create your template directly within the template record. E-mail, Fax, Letter, and PDF templates are created or uploaded on the Documents tab, under the Templates heading.
    
    You may want to include the following CRMSDK tags to include personalized information for customers who are past due:
    
    -   **NLBALANCE** - replaced with the customer's current balance
        
    -   **NLOVERDUEBALANCE** - replaced with the customer's balance that is past its due date
        
    -   **NLDAYSOVERDUE** - replaced with the number of days since the overdue balance was due
        
    -   **NLTRANID** - replaced with the transaction number
        
    
    If you use the Consolidated Payments feature, you can show consolidated balance information on the template with the following tags:
    
    -   **NLCONSOLBALANCE** - replaced with the consolidated balance for the entire customer-subcustomer hierarchy.
        
    -   **NLCONSOLOVERDUEBALANCE** - replaced with the consolidated overdue balance
        
    -   **NLCONSOLDAYSOVERDUE** - replaced with the consolidated days overdue
        
    
    For more transaction-related tags, see [CRMSDK Tags for Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N515605.html#bridgehead_N521522).
    
    If you use the Subscription Categories feature, your collection email templates should have the Subscription field on the Marketing subtab set to Billing Communication or another subscription category you created for this kind of message.
    
    For more information, see [Using Letter Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N525773.html), [Using Fax Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N529539.html), [Using PDF Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N530499.html) or [Working with Email Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N514744.html).
    
8.  Create a bulk merge to send or create all collection notices at _Documents > Mail Merge > Bulk Merge_.
    
    Note:
    
    For e-mail merges, you can generate and attach statements for each customer to illustrate which orders are overdue. On the Bulk Merge - E-mail page, check the Include Statement box on the Attachments subtab.
    

For more information, see [Merging Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N524089.html), [Merging Letters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N525062.html), [Merging Faxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N527062.html), or [Merging PDFs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N530117.html).

### Related Topics

-   [Using CRMSDK Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N515605.html)
-   [Sending Individual Collection Letters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1302583.html)
-   [Viewing Overdue Balances on the Customer Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1302769.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
