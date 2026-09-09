---
id: "section_N2470797"
type: "section"
title: "Using Multiple PayPal Accounts on Web Stores"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Web Store Transactions > Payment Options for Commerce Web Stores > PayPal Integration and Express Checkout for Commerce Web Stores > Using Multiple PayPal Accounts on Web Stores"
parent: "section_N2470255"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2470797.html"
anchors: ["procedure_N2470818"]
sha256: "b7085879fb8ef0ad62b5b9dea49466f4016390ad1a59faa0535874621b18ccca"
---

You can use a separate PayPal account for each website you operate. If you use NetSuite OneWorld, you can use a separate PayPal account for each of your subsidiaries.

#### To set up multiple PayPal accounts: {#procedure_N2470818}

1.  If you don't already have a PayPal merchant account, go to [PayPal](https://www.paypal.com/webapps/mpp/merchant) to set one up.
    
    In NetSuite, you can go to Setup > Accounting > PayPal Accounts > New and click the link near the top of the page. This link redirects you to the PayPal Business website
    
2.  Enter the following information in the Account Basics area:
    
    -   **Account Name** - Enter a name for the PayPal payment method.
        
    -   **Primary PayPal Email Address** - Enter the email address you use to log in to your PayPal merchant account.
        
        Important:
        
        To receive customer payments, your primary email address must match your merchant account email (it's case sensitive). Log in to PayPal and check your profile if needed.
        
    -   Check **Test Mode** if you're using PayPal sandbox environment for testing.
        
    -   Check **Inactive** if you don't want this PayPal account available on your website.
        
    -   Check **Use Express Checkout** to use PayPal Express Checkout on your Commerce website. Follow the instructions in [Setting Up PayPal Express Checkout for Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2470380.html) if you want to use PayPal Express Checkout.
        
    -   Check **Use Express Checkout With Bill Me Later** to let customers pay with PayPal Credit. Follow the instructions in [Setting Up PayPal Express Checkout for Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2470380.html) if you want to use PayPal Express Checkout.
        
3.  In the Payment Method area, complete the following steps to select an account for PayPal transactions:
    
    -   Select your subsidiary from the **Subsidiary** list.
        
    -   Check **Deposit To**.
        
    -   Select PayPal from the **Account** list.
        
4.  Click **Submit**.
    
    Note:
    
    PayPal integration is validated when you click **Save** on the PayPal Accounts page.
    
5.  Repeat Steps 2 through 4 for each of your PayPal accounts.
    
6.  Go to Commerce > Websites > Website List to associate your PayPal accounts with multiple websites or multiple subsidiaries in a OneWorld account. Follow these steps:
    
    -   **For multiple websites** - Go to the **Setup** subtab and select the appropriate PayPal account in the Preferences section.
        
        ![select Paypal account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Commerce/StoreFront/Transactions/WebSiteSetup_MultiPayPal_MultiSiteRedwood.png)
    -   **For OneWorld** - Go to the **Setup** subtab and associate a PayPal account record with each subsidiary.
        
        ![associate PayPal account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Commerce/StoreFront/Transactions/WebSiteSetup_MultiPayPal_SubsidRedwood.png)
7.  Click **Save**.
    

After you set up multiple PayPal accounts in NetSuite, you can track sales orders from multiple websites or subsidiaries.

### Related Topics

-   [PayPal Integration and Express Checkout for Commerce Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2470255.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
