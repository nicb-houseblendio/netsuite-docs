---
id: "section_N2245916"
type: "section"
title: "Selling Gift Certificates"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Gift Certificates > Selling Gift Certificates"
parent: "section_N2244991"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2245916.html"
anchors: ["procedure_N2245946", "procedure_N2246173", "bridgehead_N2246261"]
sha256: "abdb8349789cc76f74c6c77fa9a786859648457722abd8008275499170d882b8"
---

To sell a gift certificate, you add the gift certificate as an item on a sales transaction.

Note:

If you operate a web store, you mark the gift certificate item to display on your website. Shoppers can add the gift certificate to their carts as they would any other item and proceed to checkout. Customers who purchase gift certificates must provide the name and email address of the recipient. The recipient of a gift certificate receives an email with the authentication code they use to apply the gift certificate to an order.

#### To sell a gift certificate on a transaction entered by a sales representative: {#procedure_N2245946}

1.  Go to Transactions > Sales.
    
2.  Enter a cash sale or create a sales order.
    
3.  In the **Customer** field, select the customer you are selling the gift certificate to.
    
4.  In the **Items** list, select your gift certificate.
    
    1.  Click in the **Gift Certificate** column to fill in the following information:
        
        **From** - The name of the person, the gift certificate is from.
        
        **Recipient Name** - The name of the person receiving the gift certificate.
        
        **Recipient Email** - Enter the email for the person receiving the gift certificate. This is required so that the recipient receives the gift certificate authentication code.
        
        **Gift Message** - Enter a message for the gift certificate recipient.
        
    2.  Click **Done** to close the popup window.
        
    3.  Click **Add** to add the gift certificate to the **Item** list.
        
    
    Note:
    
    You can enter a maximum of 1 gift certificate on a transaction line. Each gift certificate line item can't have a quantity greater than 1. The details (such as From, To, Email, and Message) can be entered for only one gift certificate on a single line.
    
5.  Click the **Billing** subtab to enter payment information.
    
6.  If you entered a credit card, check the **Charge Credit Card** box.
    
7.  Click **Save**.
    

An email with the gift certificate authentication code is automatically sent to the gift certificate recipient when you save a cash sale transaction.

On sales orders or invoices, the authentication code is not sent to the recipient until the transaction is billed.

#### To confirm that a gift certificate authentication code is active: {#procedure_N2246173}

1.  Go to _Lists > Accounting > Gift Certificates_.
    
2.  If the **Remaining Value** column is blank for a gift certificate, it means the authentication code is not yet active.
    
3.  To activate the gift certificate, bill the order.
    
    1.  To find the transaction that was used to purchase the gift certificate, click on the gift certificate.
        
    2.  The transaction displays in the list.
        
    3.  Click on the transaction number to bill it.
        

For more information about viewing gift certificates, see [Viewing and Editing Gift Certificate Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2246379.html).

## Fulfillable/Receivable Status {#bridgehead_N2246261}

When you use the Advanced Billing and Advanced Shipping features, note the following. You can set a permanent status on gift certificate item records that enables or disables them to be fulfilled or received. Then, order processing is based on the fulfillable/receivable status of the item.

To set the status for each gift certificate item, check or clear the Can be Fulfilled/Received box on each item record. For more information, see [Advanced Billing and Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256787.html).

### Related Topics

-   [Enabling the Gift Certificates Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163421747294.html)
-   [Setting Preferences for Gift Certificate Authentication Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2245256.html)
-   [Creating Gift Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163421853651.html)
-   [Viewing and Editing Gift Certificate Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2246379.html)
-   [Applying Multiple Gift Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2247714.html)
-   [Gift Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2244991.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
