---
id: "section_N2653735"
type: "section"
title: "Working with Google Analytics"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Website Reports and Analytics > Using Tracking Pixels for Analytics > Working with Google Analytics"
parent: "section_N2653608"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2653735.html"
anchors: ["procedure_N2653747"]
sha256: "5d19b4a72390d6ea0b3584e3f07a4100057086fa5e12220e8c03dea087d8aee0"
---

Important:

Google Analytics 4 (GA4) has replaced Google Universal Analytics (GAU) as Google's cross-platform Analytics solution. All standard GUA properties stopped processing new hits on July 1, 2023. 360 Universal Analytics properties will stop processing new hits on July 1, 2024. GA4 is not supported on Site Builder websites..

Google Analytics is a third-party analytics solution helps evaluate traffic on your website using data based on visitor tracking information. You can use this information to optimize site content and ad campaigns.

Important:

Procedures for setting up and using Google Analytics as described in this section do **NOT** apply when configuring Google Analytics for Advanced Commerce Web Sites using the **Reference Implementations**.

#### To integrate your NetSuite website with Google Analytics: {#procedure_N2653747}

1.  Prerequisite steps:
    
    1.  Create your own account with **Google Analytics**. For more information, visit the [Google Analytics Web site](http://www.google.com/analytics).
        
    2.  In **Google Analytics**, add a profile for the domain you want to track.
        
    3.  On the **Standard** tab, select multiple top-level domains.
        
    4.  Copy the tracking pixel code provided for you by Google Analytics.
        
    5.  Click **Save** and **Finish**.
        
    6.  In the **Website Profiles** list, click **Edit** next to the profile you want to enable.
        
    7.  On the Profile Settings page, click **Edit** next to **Main Website Profile Information**.
        
    8.  Set the **E-Commerce Website** radio button to **Yes**.
        
    9.  Click **Save Changes**.
        
2.  Log in to NetSuite.
    
3.  Go to _Commerce > Websites > Website List_ and click Edit next to the website name. Click the **Analytics** subtab to enter your tracking snippet, along with HTML code and website tags for tracking analytics data.
    
    Important:
    
    If you have a hosted site, paste your Google Analytics tracking snippet in your hosted HTML pages. Then, enter custom analytics tracking code in the **Analytics Click Attributes**, **Analytics Submit Attributes**, and **Order Tracking Script HTML** fields. When you do this, website tags you use to create links to forms and checkout pages will collect tracking data across domains.
    
    1.  **Addition to <head>** - Paste your Google Analytics tracking snippet in this field. Your tracking code is then added to every page of your NetSuite-generated site.
        
        For example:
        
                            `<script type="text/javascript">     var _gaq = _gaq || [];   _gaq.push(['_setAccount', 'UA-12345678-9]);   _gaq.push(['_setDomainName', 'none']);   _gaq.push(['_setAllowLinker', true]);   _gaq.push(['_trackPageview']);     (function() {     var ga = document.createElement('script'); ga.type = 'text/javascript'; ga.async = true;     ga.src = ('https:' == document.location.protocol ? 'https://ssl' : 'http://www') + '.google-analytics.com/ga.js';     var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(ga, s);   })();   </script>` 
                          
        
    2.  **Analytics Click Attributes** - Add attributes for the Add To Cart button. The code in this field modifies link URLs by adding your tracking pixel. This applies to links for registration, checkout, and any other links that go to checkout pages. Use this syntax:
        
                            `onclick="if(typeof(_gaq._getAsyncTracker) == 'undefined') { return true; } else { _gaq.push(['_link', this.href]); return false; }"` 
                          
        
    3.  **Analytics Submit Attributes** - Add attributes for the Proceed to Checkout button. Code in this field captures analytics data when shoppers go to checkout from the shopping cart, and when they submit forms on your website. Use this syntax:
        
                            `onsubmit="_gaq.push(['_linkByPost', this]); return true;"` 
                          
        
    4.  **Order Tracking Script HTML** - Code in this field, is applied to the order confirmation page, or Thank You page, that displays after a shopper submits a Web order on your site. You can use the sample code provided below to get started. Replace the account number in the sample, with your own Google Analytics account number:
        
                            `<script type="text/javascript">     var _gaq = _gaq || [];   _gaq.push(['_setAccount', 'UA-12345678-9']);   _gaq.push(['_setDomainName', 'none']);   _gaq.push(['_setAllowLinker', true]);    _gaq.push(['_addTrans',         "<%=getCurrentAttribute('confirmation','ordernumber')%>",               "<%=getCurrentAttribute('site','name')%>",      "<%=getCurrentAttribute('confirmation','subtotal')%>",              "<%=getCurrentAttribute('confirmation','tax')%>",               "<%=getCurrentAttribute('confirmation','shipping')%>",         "<%=getCurrentAttribute('confirmation','shiptocity')%>",        "<%=getCurrentAttribute('confirmation','shiptostate')%>",          "<%=getCurrentAttribute('confirmation','shiptocountry')%>"]);        var itemsInOrder = "<%=getCurrentAttribute('confirmation','orderitems')%>";    var lineItem = itemsInOrder.split("||");    for(var inum = 0; inum < lineItem.length; inum++)  {  var itemAttributes = lineItem[inum].split("|");  _gaq.push(['_addItem',           "<%=getCurrentAttribute('confirmation','ordernumber')%>",               itemAttributes[0],                     itemAttributes[1],                     itemAttributes[2],                  itemAttributes[3],             itemAttributes[4]]);    }        _gaq.push(['_trackTrans']);      (function() {     var ga = document.createElement('script'); ga.type = 'text/javascript'; ga.async = true;     ga.src = ('https:' == document.location.protocol ? 'https://ssl' : 'http://www') + '.google-analytics.com/ga.js';     var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(ga, s);   })();   </script>` 
                          
        
        For more information about the website tags you can use in this field, see [Order Confirmation Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627572.html).
        
4.  Check the **Enable Google Analytics Integration** box.
    
    Check this box to pass Google tracking cookies from shopping to checkout. This along with the fields on the Analytics subtab are required for cross-domain analytics tracking to integrate NetSuite with your Google Analytics account. Clear this box if Google Analytics Integration interferes with a custom solution you have already implemented for cross-domain tracking.
    
5.  Click **Save**.
    

After adding your tracking code to the site, you can verify data is being captured on the order confirmation page. Place a test order, and then on the Thank You page, select View Source from the View menu in the browser. You should see values for each tag included in the script you added to the Order Script Tracking HTML field.

You can also use website tags for tracking visitor information about the checkout tab. For more information, see [Checkout Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627341.html).

### Related Topics

-   [Web Analytics and Online Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2654243.html)
-   [Using Tracking Pixels for Analytics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2653608.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
