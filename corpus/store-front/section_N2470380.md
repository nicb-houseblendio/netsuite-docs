---
id: "section_N2470380"
type: "section"
title: "Setting Up PayPal Express Checkout for Web Stores"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Web Store Transactions > Payment Options for Commerce Web Stores > PayPal Integration and Express Checkout for Commerce Web Stores > Setting Up PayPal Express Checkout for Web Stores"
parent: "section_N2470255"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2470380.html"
anchors: ["procedure_N2470395"]
sha256: "d245c113ea128e06216657fab80db4f1f92d4ed00fc930f267774bc1650528a1"
---

PayPal Express Checkout lets your customers check out using information saved in their PayPal accounts without having to re-renter details on your website. You can take advantage of PayPal and partner offers using Express Checkout. After integrating PayPal Express Checkout with NetSuite, you can issue returns through PayPal.

After you set up PayPal Express Checkout, customers click the PayPal button in your shopping cart, get redirected to PayPal to confirm or change their details, then return to your site to enter any gift certificates or coupon codes and to submit the order.

Note:

Customers need a PayPal account to complete payment with PayPal Express Checkout.

Complete the following tasks to set up PayPal Express Checkout in NetSuite:

-   Set up your PayPal merchant account with API access to NetSuite transactions.
    
-   Set up PayPal Express Checkout in NetSuite.
    

#### To set up your PayPal account with API access to NetSuite transactions:

1.  If you don't have a PayPal merchant account, go to [PayPal](https://www.paypal.com/webapps/mpp/merchant) to set one up.
    
    In NetSuite, you can go to Setup > Accounting > PayPal Accounts > New and click the link near the top of the page. This link redirects you to the PayPal Business website.
    
    Important:
    
    Your PayPal account needs to be Premier or Business to set up the required API access for PayPal Express Checkout.
    
2.  Log in to your PayPal merchant account and, depending on your environment, use one of the following API usernames for granting API Access to NetSuite:
    
    -   For production accounts - **ppexpresscheckout\_api1.netsuite.com**
        
    -   For sandbox or demo accounts - **dwilli\_1183500510\_biz\_api1.netsuite.com**
        
3.  Check the following options in the list of APIs:
    
    -   Use Express Checkout to process payments.
        
    -   Issue a refund for a specific transaction.
        
    -   Obtain information about a single transaction.
        
    -   Search your transactions for items that match specific criteria and display the results.
        
    -   Authorize and capture your PayPal transactions.
        

#### To set up PayPal Express Checkout in NetSuite: {#procedure_N2470395}

1.  Confirm the PayPal Integration feature is enabled in NetSuite.
    
    Go to Setup > Company > Enable Features.
    
2.  Click the **Transactions** subtab.
    
3.  In the Payment Processing area, check the **PayPal Integration** box to enable PayPal as a payment method on your Commerce website.
    
4.  Click **Save**.
    
5.  Create a PayPal account record in NetSuite that corresponds with your PayPal account.
    
    Go to Setup > Accounting > PayPal Accounts > New.
    
6.  Enter the following information in the Account Basics area:
    
    -   **Account Name** Enter a name for the PayPal payment method.
        
    -   **Primary PayPal Email Address** - Enter the email address you use to log in to your PayPal merchant account.
        
        Important:
        
        To receive customer payments, your primary email address must match your merchant account email (it's case sensitive). Log in to PayPal and check your profile if needed.
        
    -   Check **Test Mode** if you're using PayPal sandbox environment for testing.
        
    -   Check **Inactive** if you don't want this PayPal account available on your website.
        
    -   Check **Use** **Express Checkout** to use PayPal Express Checkout in your Commerce website. Follow the instructions in [Setting Up PayPal Express Checkout for Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2470380.html) if you want to use PayPal Express Checkout
        
        Important:
        
        You'll need to set up API access in your PayPal Express merchant account to enable integration with NetSuite.
        
    -   Check **Use Express Checkout With Bill Me Later** to let customers pay with PayPal Credit.
        
7.  In the Payment Method area, complete the following steps to select an account for PayPal transactions:
    
    -   Select your subsidiary from the **Subsidiary** list.
        
        Note:
        
        The subsidiary must be the same as the one you select in Step 12.
        
    -   Check **Deposit To**.
        
    -   Select PayPal from the **Account** list.
        
8.  Click **Submit**.
    
    Note:
    
    PayPal integration is validated when you click Save on the PayPal Accounts page. If PayPal Express Checkout is set up correctly, the page saves successfully.
    
9.  Go to Commerce > Websites > Website List to associate your PayPal account with your subsidiary.
    
10.  Click **Edit** next to the name of your website.
     
11.  Go to the **Setup** tab.
     
12.  At the bottom of the **Setup** tab, in the Subsidiaries area, go to the row for your subsidiary and select your PayPal account from the PayPal Account list.
     
     Note:
     
     The subsidiary must be the same as the one you selected in Step 7.
     
13.  Click **Save**.
     

To associate multiple PayPal accounts with your NetSuite account, see [Using Multiple PayPal Accounts on Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2470797.html).

When a customer completes checkout, NetSuite creates a sales order with payment authorized by PayPal. Depending on your accounting settings, the sales order status in NetSuite is either Pending Fulfillment or Pending Approval. After the order is billed, payment is received from PayPal.

Note:

NetSuite doesn't send an email if the order can't be processed. If there's a funding issue in PayPal, the customer goes back to PayPal, sees the error, and can pick a new funding source to resubmit the order.

If you don't want to use Express Checkout, don't check the **Use Express Checkout** box unchecked when you enable the PayPal Integration feature in NetSuite. Customers can still choose PayPal as a payment option at checkout. Fore details, see [Web Store PayPal Integration Without Express Checkout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2473756.html).

### Related Topics

-   [PayPal Integration and Express Checkout for Commerce Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2470255.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
