---
id: "section_N1292421"
type: "section"
title: "Creating a Payment Method"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Customer Payments > Creating a Payment Method"
parent: "section_N1285644"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1292421.html"
anchors: ["procedure_N1292443", "bridgehead_4592579952", "bridgehead_161282561381", "bridgehead_4592542463", "bridgehead_4592548149", "bridgehead_4291042820"]
sha256: "b5284ef64b9f31824b9d99c2ed757e7fe55c438e358bf256736a9d12ddc03c62"
---

A payment method represents an account that transactions write into.

With a payment method, you can:

-   configure an account
    
-   determine how payment processing is performed
    

You can also use payment methods when configuring payment processing profiles.

#### To create a payment method: {#procedure_N1292443}

1.  Go to _Setup > Accounting > Setup Tasks > Accounting Lists > New_ , then select the **Payment Method** Type from the drop-down list in the **Filters** section, and then click **New**.
    
2.  Enter a name for the payment method in the **Name** field.
    
    If you are creating a payment card payment method, see [Accepted Names for Payment Card Payment Methods](#bridgehead_4592542463) for a list of accepted names.
    
3.  Select the **Type** of the Payment Method from the drop-down list:
    
    -   **ACH** - an online payment method that requires the [Payment Instruments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1538492538.html) feature to be enabled. The method requires a token that was issued by a payment gateway and does not represent a bank account. The ACH payment instrument only works with the ACH payment method. The methodtype field value ID is 13.
        
    -   **EMV** - an online payment method that is specific to the EMV Chip and PIN flow for point of sale (POS) solutions. The EMV payment method type usually supports Sale and Refund operations, and requires a special device to initiate payment operations. The methodtype field value ID is 5.
        
    -   **External Checkout** - an online payment method that is used in E-Commerce. The shopper is redirected to an external payment provider's page to authorize the payment and generate the sales order. Merchants can import sales orders by using only the P/N Ref identifier. For details, see the help topic [Importing Sales Orders with P/N Ref Identifiers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158385280263.html). The methodtype field value ID is 6.
        
    -   **General Token** - an online payment method that requires the [Payment Instruments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1538492538.html) feature to be enabled. The method requires a token that was issued by a payment gateway and does not represent a payment card. The General Token payment instrument, only works with the General Token payment method. The methodtype field value ID is 2.
        
    -   **Offline** - the payment happens outside of NetSuite, for example a cash transaction. The methodtype field value ID is 9.
        
    -   **Pay By Reference** - an online payment method that requires the [Payment Instruments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1538492538.html) feature. The method uses a payment reference issued by a payment gateway integration to perform a follow-up operation.
        
        Certain integrations do not share tokens, but can share a transaction reference. You can use the reference to, for example, capture after authorization without having a payment instrument or a payment card number. Or you can perform a referenced refund without the original credentials.
        
        You cannot select the Pay By Reference payment method type on transactions where neither capture nor refund is available.
        
        The methodtype field value ID is 10.
        
    -   **Payment Card** - an online payment method for common card processing. The method supports both Mail Order / Telephone Order (MOTO) and e-commerce payments. The methodtype field value ID is 1.
        
    -   **Payment Card Swipe** - an online payment method for card present processing. Using the method requires a special device to read a magnetic card stripe. The methodtype field value ID is 4.
        
    
    -   **Payment Card Token** - an online payment method for card processing with tokenization. The method processes tokens instead of payment cards. The methodtype field value ID is 3.
        
4.  Check the **Display in Web Site** box to use this payment method on your web store.
    
5.  Check the **External Checkout** box if this payment method requires that your web store customers check out on a third-party website.
    
    For more information, see [Alternative Non-Credit Card Payment Methods for Web Store Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4213266422.html)
    
6.  Check the **Requires Line-Level Data** box if you want details of all line items to be always sent to the payment gateway when this payment method is selected on a transaction.
    
7.  On the **Account** subtab, select one of the following:
    
    1.  **Group with Undeposited Funds**. Select this option to batch payments prior to deposit into a bank account and entry into a general ledger account. Group with Undeposited Funds set on a payment method takes precedence over the Account field on a transaction. A transaction will be processed with the Undeposited Funds account even if you select another account on the transaction.
        
    2.  **Deposit To**. Select this option and then select a bank account from the drop-down list in the **Account** field.
        
    
    For more information about how the settings you choose for the payment method determine how NetSuite posts payments, see [The Effect of Payment Method Settings on Funds Posting](#bridgehead_4592548149).
    
8.  On the **Payment Visuals** subtab, choose which images show for this payment method on the web store checkout page as follows:
    
    1.  In the **Flags** column, enter the flag used to reference this image on your site.
        
        If you are using a SiteBuilder website, enter **web/standard**. If you are using a SuiteCommerce Advanced site, you can use any flag used in the code on your site.
        
        Note:
        
        If you enter more than one image with the same flag, each one of those images shows on websites that use this payment method.
        
    2.  In the **URL** column, paste the URL for the image you want to use for this payment method. See [NetSuite Default URLs for Major Payment Methods](#bridgehead_4291042820) for a list of default URLs.
        
    
    Warning:
    
    If you do not enter an image for at least one of your web store payment methods, the following error message shows on the payment information page: Payment Method: Unable to Proceed. This business does not have any external payment methods defined.
    
9.  Click **Save**.
    

## Restricting Web Store Payment Methods by Customer Currency {#bridgehead_4592579952}

If you want to only show those payment methods that support the shopper's currency on the payment page of your web store, go to Commerce > Websites > Website List. On the Shopping subtab, under Payments Page, check the **Restrict Payment Methods by Customer Currency** box. This prevents payment processing profiles that are not compatible with the customer's currency from appearing on the checkout payment page.

## Restricting Web Store Payment Methods by Country of Shipping Address {#bridgehead_161282561381}

If you want to only show those payment methods that support the country of the shipping address on the payment page of your web store, go to Commerce > Websites > Website List. On the Shopping subtab, under Payments Page, check the **Restrict Payment Methods by Country of Shipping Address** box. This prevents payment processing profiles that are not compatible with the country of the shipping address from appearing on the checkout payment page.

## Accepted Names for Payment Card Payment Methods {#bridgehead_4592542463}

The name of a payment card payment method must identify the type of credit card. Use the names in the following list when you create a credit card payment method:

-   Visa
    
-   Master Card
    
-   MasterCard
    
-   Amex
    
-   American Express
    
-   AmericanExpress
    
-   Discover
    
-   Diners Club
    
-   DinersClub
    
-   JCB
    
-   Switch
    
-   Maestro
    
-   Solo
    
-   Laser
    

Note:

These names are not case sensitive.

## The Effect of Payment Method Settings on Funds Posting {#bridgehead_4592548149}

The following table describes how you can set up your payment methods to determine where funds are posted.

| Settings on the payment method record | Where transaction payment funds post |
| --- | --- |
| Select Deposit To. and Select \[Settlement Account\] in the Account field. | Payments post to the general ledger account selected on the merchant bank account record. |
| Select Deposit To. and Select any general ledger account **other than** \[Settlement Account\] in the Account field. | Payments post to the general ledger account, of the Bank type, selected in the Account field. |
| Select Undeposited Funds. | Payment funds post to Undeposited Funds. |

## NetSuite Default URLs for Major Payment Methods {#bridgehead_4291042820}

The following table lists NetSuite default URLs for major payment methods. You **must** type these URLs manually in the URL field.

Important:

Copying and pasting these URLs causes an error and prevents the icon image from displaying. Instead, manually type these URLs.

| Payment Method | URL |
| --- | --- |
| Visa | /images/icons/creditcard/pmt\_visa.gif |
| Master Card | /images/icons/creditcard/pmt\_mc.gif |
| Discover | /images/icons/creditcard/pmt\_discover.gif |
| American Express | /images/icons/creditcard/pmt\_amex.gif |
| Cash | /images/icons/creditcard/pmt\_other.gif |

Important:

To show the image of a local credit card payment method, upload the image to NetSuite File Cabinet. Then, enter the link of this image in the URL column on the Payment Visuals subtab of this payment method. Make sure the image record in the file cabinet is externally available.

### Related Topics:

-   [Accepting Customer Payments Workflow Chart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1285644.html#section_N1288273)
-   [Applying a Payment on the Customer Payment Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1288824.html)
-   [Applying a Payment on an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1289458.html)
-   [Correcting Payments to Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1292877.html)
-   [Entering Payment Information on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586835857.html)
-   [Removing Credits from Deleted Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1292961.html)
-   [Reversing or Deleting Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4744566376.html)
-   [Approving Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4373987935.html)
-   [Managing Undeposited Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1294497.html)
-   [Consolidated Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1288474.html)
-   [Payment Receipts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1293235.html)
-   [Creating a Payment Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1292421.html)
-   [Handling Returned/NSF Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1295030.html)
-   [Allowing Customers to Pay Online](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1293669.html)
-   [Set Up Credit Card Payments for Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2469773.html)
-   [Importing Sales Orders with P/N Ref Identifiers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158385280263.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
