---
id: "chapter_N3920840"
type: "chapter"
title: "FAQ: Site Builder Website"
branch: "frequently-asked-questions"
category: "additional-resources"
breadcrumb: "Additional Resources > Frequently Asked Questions > FAQ: Site Builder Website"
parent: "book_N3895042"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3920840.html"
anchors: ["question_N3920861", "question_N3921132", "question_N3921330", "question_N3922726", "question_N3922973", "procedure_N3922986", "procedure_N30130221", "question_N3923188", "bridgehead_N3923268", "question_N3923302", "procedure_N3923320", "question_N3923554", "question_N3923747", "question_N3924013", "question_N3924141", "question_N3924119", "question_N3923602", "question_N3924195", "question_N3924354", "question_N3924379", "question_N3924402", "question_N3924474", "question_N3924513", "question_N3924573", "question_N3924622", "question_N3924715", "question_4090082967"]
sha256: "bff0a6700696f5c31425bfcbb8ac5611e05e1c8bd10a221ddfc9ff09f553fa45"
---

See the questions and answers below for information about Site Builder websites.

### How do I point a domain to my NetSuite website? {#question_N3920861}

NetSuite recommends using a CNAME redirect to point your custom shopping domain at your NetSuite website. This is applicable to both Site builder and SuiteCommerce Advanced websites Using a CNAME is the best way to integrate your domain. For more information, see [Point Your Domain Name at Your Domain (DNS Settings)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2479403.html).

See the following topics.

-   [Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2478982.html)
    
-   [Point Your Domain Name at Your Domain (DNS Settings)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2479403.html)
    
-   [Link a Checkout Domain with Your Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157953243614.html)
    

### How do I add custom fields to my website? {#question_N3921132}

When you create custom fields for your website, you must check both the **Web Site** box and the **Sales** or **Customer:Projects** box to have your fields appear both in your website and on your sales transactions or customer records.

Note:

The availability of these custom field types depends on the NetSuite product you use. For more information, contact your account manager.

-   Entity fields can be placed on customer records and in the registration form of your website. On the Custom Entity Field page, on the **Applies To** subab, be sure to check the **Customer:Projects** box.
    
-   Transaction body fields can be placed on sales transactions and in the checkout area of your website. On the Transaction Body Field record on the **Applies To** subtab, check both the **Sale** box and the **Web Store** box. The field is displayed on the last page of the web store checkout process.
    
    Transaction body fields are only useful when you operate a full Web store, that uses the NetSuite shopping cart and checkout.
    
-   Transaction column fields can be placed on sales transactions and with each item listed in your website. On the Transaction Column Field Form, check the boxes for both **Sale Item** and **Store Item**.
    
-   Transaction item options can be placed on sales transactions and with each item listed in your website. On the Item Option page, on the **Applies To** subtab, check the boxes for both **Sale** and **Web Store**.
    

If you only check the Sale or Customer:Projects box for custom fields, the field appears only on your sales transactions or customer records. It does not appear in your website.

If you only mark the Web Store or Store Item box for custom fields, the field appears in your website, but the information collected does not appear on the sales transactions or customer records that are created from your website.

Unless you mark both boxes, the information collected from your website is lost.

See the following topics.

-   [Customizing the Website Registration Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2578016.html)
    
-   [Creating Custom Entity Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827562.html)
    
-   [Creating Custom Transaction Body Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828059.html)
    
-   [Creating Custom Transaction Line Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828307.html)
    
-   [Creating Custom Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828730.html)
    

### Why aren't images showing correctly in my web store? {#question_N3921330}

In your web store, if you see a missing image icon instead of your image, please check the following:

1.  Make sure that the image you are trying to reference is located in the Images folder of your file cabinet.
    
2.  Make sure it is a valid image file. Try downloading the image to your desktop and viewing the image.
    
3.  Make sure the Available Without Login box is marked:
    
    1.  In NetSuite, click the Documents tab.
        
    2.  Click the Images folder.
        
    3.  Click Edit next to the image in question.
        
    4.  Check the Available Without Login box.
        
    5.  Click Save.
        
4.  Make sure you are using the correct URL to reference the image:
    
    1.  Click the Documents tab.
        
    2.  Click the Images folder.
        
    3.  Click Edit next to the image in question.
        
    4.  Make sure you are referencing the first URL listed that begins with **http://shopping.netsuite.com**.
        

If you continue to experience a problems viewing your image, please contact Technical Support.

See the following topics.

-   [Images](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2592452.html)
    
-   [Using Images in your Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2592719.html)
    
-   [Resizing Images](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2594819.html)
    

### How do I set up an external catalog site? {#question_N3922726}

To turn on the External Catalog Site feature, go to _Setup > Company > Setup Tasks > Enable Features_. On the Web Presence tab, check the box for External Catalog Site (WSDK), and click Save.

To set up an external catalog site, you first need to make sure your items are available online. If your items are not available online, then these items cannot be integrated with your website.

For more information, read [External Catalog Site (WSDK) Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2600392.html), and [Setting Up an External Catalog Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2600712.html).

### Why is a matrix item not appearing in my web store? {#question_N3922973}

If you have set up a matrix item but it is not appearing in your web store, it could be because you have not setup a Transaction Item Option for each of the custom lists associated with the matrix item.

#### To create a transaction item option: {#procedure_N3922986}

1.  Go to _Customization > Lists, Records, & Fields > Transaction Item Options > New_.
    
2.  Enter a name for the field in the **Label** field.
    
3.  In the **Type** field, select **List/Record**.
    
4.  Select your custom list in the **List/Record** field.
    
5.  On the **Applies To** tab, check the **Web Store** box.
    
6.  In the **Items** field, select each matrix parent item that your custom list is associated with and that you want to appear in your web store.
    
7.  Click on the **Sourcing & Filtering** tab.
    
8.  In the **Source List** field, select **Item**.
    
9.  In the **Source From** field, select your custom item field that is used to set up this matrix option.
    
10.  Click **Save**.
     

If you have set up the Transaction Item Option fields for the matrix item, and the matrix item still does not display on the website; the problem may be that the matrix item is not selected on the Transaction Item Option Record.

#### To confirm a transaction item option is set up correctly for a matrix item: {#procedure_N30130221}

1.  Go to _Customization > Lists, Records, & Fields > Transaction Item Options > New_.
    
2.  Click on the **Item Option** you want to confirm.
    
3.  On the **Applies To** subtab, confirm that the name of the matrix item is displayed in the Items field.
    
4.  If the matrix item is not displayed, add it to the Items field.
    
5.  Click **Save**.
    

If your matrix item has been properly setup it should now display in your web store. For more information aboutmatrix items please click Help in the upper right hand corner of your NetSuite account and enter Matrix Item in the Search field.

See the following topics.

-   [Using Transaction Line Fields in Your Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2586257.html)
    
-   [Using the Matrix Item Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227918.html)
    

### How do I prevent secure and not secure item warnings from popping up in my website? {#question_N3923188}

## To resolve the problem by changing the HTML on your page: {#bridgehead_N3923268}

You can prevent the secure and nonsecure items warnings from displaying on your site by using relative URLs to refer to images displayed on secure pages.

For example, use **<IMG SRC="https://docs.oracle.com/images/small\_logo.gif">** instead of **<IMG SRC="http://shopping.netsuite.com/images/small\_logo.gif">.**

### How can I make a logo image show as a favicon? {#question_N3923302}

When you save a logo with the file extension .ico, you can have a favicon show with your site name when it is bookmarked. You must have the Advanced Site Customization feature enabled to use favicons.

#### To show a logo as a favicon: {#procedure_N3923320}

1.  Use an application such as **Icon Forge** to create and save a logo using the file extension .ico. You should save your icon with name **favicon.ico**.
    
    You must use a program that lets you save images as icons.
    
2.  Upload your favicon.ico file to the **Web Hosting Files** folder of your file cabinet.
    
    To do this, click the **Documents** tab, and go to Web Site Hosting Files > Live Hosting Files. Click **Add File** to select and add your favicon.
    
3.  Go to Setup > Web Site > Themes, and click **Customize** next to the theme you use for your site.
    
4.  Insert following in the Addition to <head> field:
    
                        `<link href="https://docs.oracle.com/favicon.ico" rel="shortcut icon" type="image/x-icon">` 
                      
    

See the following topics.

-   [Customizing Site Themes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603752.html)
    
-   [Hosting HTML Websites with NetSuite Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2598355.html)
    

### Are there limits on the number of items or categories I can have? {#question_N3923554}

There is no limit to the number of categories you can publish to your website. However, fifty categories will display on a page. Visitors to your site can click on pagination links to view all the categories on your site.

There is a limit of 1,000 items that can display in a category. Any items over the first 1,000 will be returned in search results. Up to fifty items will display on each page. Visitors to your site can click on pagination links to display all items in a category.

### Why aren't items showing on my web store? {#question_N3923747}

If the items you created are not displayed in your web store, confirm the following settings:

-   The **Display in Web Site** box is checked on the item record.
    
-   The item is published to a tab or category.
    
    -   To display the item to all shoppers on your web store, confirm the **Display in Web Site** box is checked on the tab or category record the item is published to.
        
    -   To display an item only to certain visitors, you can select a specific customer role or group on the **Audience** subtab of the tab or category record, and clear the **Display in Web Site** box.
        
    -   If the item is not published to a tab or category, check the **Show Uncategorized Items** box on the **Setup** subtab, in the Preferences section at _Commerce > Websites > New_. This way, the item displays in search results, but is not displayed on your web store.
        
    -   If you have multiple websites, confirm the item is published to the current site
        
-   A price is entered on the item record.
    
    -   Confirm the item has a default online price level.
        
    -   If the item does not have an online price level, confirm that it has an alternative price level that matches the current customer's price level.
        
-   If the item is a matrix item, confirm the following:
    
    -   The child matrix items have a price.
        
    -   The matrix item has transaction item options, and the item options are set up correctly. For more information, see [Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227654.html).
        
-   If you have a NetSuite OneWorld account, the item must be published to the subsidiaries displayed on the website.
    
-   If you have a NetSuite OneWorld account, the item must have a price in the shopper's currency or in the base currency of the subsidiary that the shopper is viewing on the website.
    
    For example: When a shopper's currency is USD, an item with no price in USD, is not displayed.
    
-   On the item record, click the Store subtab, and confirm that the Out of Stock Behavior field is NOT set to **Remove when item is out-of-stock**.
    

See the following topics.

-   [Displaying Items and Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2585301.html)
    
-   [Featuring Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2585769.html)
    
-   [Adding Items to Web Store Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2585643.html)
    
-   [Setting Web Store Back Order and Out-of-Stock Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2582357.html)
    
-   [Item Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2180614.html)
    

### What message is displayed to website visitors during NetSuite scheduled maintenance? {#question_N3924013}

You can create and upload your own HTML page to display on your site when you take your site offline for maintenance, and during NetSuite scheduled maintenance periods. First, you must set up a site maintenance folder, and then you can upload your custom HTML page into the file cabinet in NetSuite. For more information, see [Custom Maintenance Folder and Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7112636199.html).

If you choose not to create your own maintenance page, a generic message is displayed in all websites indicating to visitors that the shopping cart is not available.

The generic message displayed to web store visitors is:

_System Maintenance Period_

_Our web site is temporarily unavailable while we perform routine system maintenance. We are working on the site to improve its appearance and functionality._

_We sincerely apologize for the inconvenience. Please visit us again later._

### What price is displayed for items on my web store? {#question_N3924141}

NetSuite uses the following criteria to determine the price that displays for items in your web store:

1.  If a customer has a preferred price level set on their customer record, they will see that price when they log into the web store.
    
2.  If the item has an online price defined on the item record, the online price is displayed.
    
3.  If the item has no online price set and a base price exists, the base price is displayed.
    
4.  If all the price levels are blank on the item record, the item is not displayed in the web store.
    

### Do session IDs affect my search engine ranking? {#question_N3924119}

No. NetSuite provides pages that are free of session IDs when it detects search engine spiders. Session IDs are necessary to preserve shopping continuity on the secure NetSuite checkout server when a shopper on the web store is blocking cookies. For more information about Search Engine Optimization, see Search Engine Optimization (SEO).

### In what order are search results displayed on my website? {#question_N3923602}

When a visitor to your site runs a search, the results are presented in order of relevance. NetSuite determines relevance by matching the keywords in the visitor's search with the number of times those keywords appear on your site, and the fields in which those keywords appear.

NetSuite matches keywords using the following algorithm for ranking:

1.  Item names or keywords defined in these fields on item records display first:
    
    -   Item Name/Number
        
    -   Web Store Display Name
        
    -   Search Keywords
        
2.  Keywords in the Web Store Description field display next.
    
3.  Keywords in the Detailed Description field display last.
    

You can choose to display matches to keywords in site category names at the top of the search results list. Go to Setup > Set Up Web Site. On the Search subtab, check the **Include Categories** box.

See the following topics.

-   [Search Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591207.html)
    
-   [Helping Customers Find Items on Your Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2634841.html)
    

### Which items are displayed first in web store search results? {#question_N3924195}

Items displayed in web store search results are sorted by their overall rank as determined by which rank groups keywords fall into for each item.

Keywords in the Name and Search Keywords fields on the item record have a high rank.

-   On the Basic subtab:
    
    -   Display Name
        
    -   Item Name/Number
        
    -   Sales Description
        
-   On the Store subtab:
    
    -   Store Display Name
        
    -   Search Keywords
        
    -   Search Keywords
        

Keywords in description fields rank lower.

-   On the Basic subtab:
    
    Sales Description
    
-   On the Store subtab:
    
    -   Store Description
        
    -   Detailed Description
        
    -   Featured Description
        

Keywords in the Page Title field rank lowest.

When you run a search in the web store, all items with matching keywords are extracted and ordered by rank from highest to lowest.

### Are browser cookies required to view my web store? {#question_N3924354}

Browser cookies are required for checkout. When you integrate your website with the NetSuite shopping cart, shoppers on your website need to have cookies enabled in their browsers to complete checkout. This is consistent with industry standards. Web stores generally rely on browser cookies for authentication, storing site preferences, and storing shopping cart contents.

At key points during the shopping session, NetSuite detects when a web browser is set to block cookies and displays a message alerting the shopper that cookies are blocked. The message also provides the shopper with instructions on how to enable cookies in FireFox browser to continue with checkout on your web store.

### What is the lifespan of a web store shopper's browser cookie? {#question_N3924379}

The returning shopper is automatically recognized for up to a week. After a week the shopper must log in to see his or her shopping cart. The cart becomes abandoned if the shopper has not registered and does not return in a week using the same browser.

### What should I do if I receive an alert about an error during checkout? {#question_N3924402}

These errors typically occur because the customer made a mistake during checkout. In most cases, web store customers are able to resolve the problem, and successfully submit an order. If you do not see an order from the customer after several hours, and you notice more errors from other customers, report the error number to NetSuite Customer Support.

Email alerts can also include any of the following problems:

-   Sales order creation failure
    
-   Transaction is out of balance
    
-   Custom field error - This can occur if an item option selected for an item in the shopping cart has been deleted or inactivated since it was added to the card.
    
-   Credit card processor error
    

For more information, see [Set Website Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2572962.html).

### What is the maximum number of search results that can display on my site? {#question_N3924474}

Up to 1000 items, including categories can display in search results on your website. Note that you must select a preference to include categories in search results. For more information, see [Web Site Search Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2572319.html).

### Can visually impaired individuals use NetSuite websites with JAWS or other assistive technologies for web accessibility? {#question_N3924513}

Accessibility guidelines typically require that website designers avoid using HTML tables for arranging data on web pages. A NetSuite hosted website provides designers with full control over the HTML, whereas NetSuite-generated sites rely on HTML tables to organize content, and may not comply with accessibility guidelines.

To start creating a hosted website with NetSuite, go to Setup > Company > Enable Features. Click the Web Presence subtab, and then check the **Host HTML Files** box. For more information, see [Hosting HTML Websites with NetSuite Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2598355.html).

### How does NetSuite determine the From address in email messages sent from my web store? {#question_N3924573}

The address in the **Email From Address** field overrides the address in the **Default Web Store Email From Address** field.

If the **Default Web Store Email From Address** is blank, and you have not entered an email address for any particular email message type, then NetSuite uses the email address you entered as your company email address.

Note that if you operate multiple websites, you can set different email addresses for each site. Go to the Web Site Setup page to modify the **Email From Address** field on each site associated with your account.

### What types of email messages are sent from the web store? {#question_N3924622}

You can set preferences for when you want email messages to be sent from the web store. For more information about email preferences, see [Set Website Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2572962.html).

The following actions on your website can generate an email message. Note that you can choose which email messages to send depending on how your company processes orders:

-   When the order is received on your website.
    
-   When the sales order is approved.
    
-   When the order is Fulfilled.
    
-   When an order is canceled.
    
-   When a gift certificate has been purchased. An email is sent to the customer who purchased the gift certificate, and to the recipient.
    
-   When a file is available for download.
    
-   When a license code is available for a downloadable item, such as a software download.
    

In addition to the messages listed above, you can choose to receive an email message alert if an error occurs at checkout that prevents a customer from submitting an order.

### How can my web store retrieve a shopper's email and name when the shopper is recognized but is not logged in? {#question_N3924715}

When a shopper is not logged in, web store scripts may not have access to the shopper's NetSuite customer record that has the email and name. If the shopper is recognized, scripts can instead use the nlObjContext getEmail() and getName() methods to return the shopper's email and name. For information about these methods, see [nlobjContext](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4752730521.html#bridgehead_4726863209).

### How long before the reset password link expires for my web store customers? {#question_4090082967}

The password recovery link expires in one hour. NetSuite provides a tag that generates the password recovery link URL. You can include the tag in an email message template. For more information, see [Web Store Password Recovery Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2573247.html#bridgehead_N2574603).

### I'm seeing a lot of 503 Service Unavailable errors on my website. How are these errors generated?

IP address blocking is used to protect against attacks from malicious web crawlers. NetSuite blocks IP addresses by sending a 503 error if the user-agent is not recognized, or if there are too many requests being made. For example, an unrecognized crawler attempting to download a site faster than a page every few seconds may be flagged as potentially malicious or abusive.

Note that NetSuite keeps a list of approved user agents such as Google and other approved search bots. Trusted crawlers do not make requests abusively.

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
