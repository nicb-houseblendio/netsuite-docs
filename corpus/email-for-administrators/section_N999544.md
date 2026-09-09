---
id: "section_N999544"
type: "section"
title: "DomainKeys Identified Mail (DKIM)"
branch: "email-for-administrators"
category: "account-administration"
breadcrumb: "Account Administration > Email for Administrators > DomainKeys Identified Mail (DKIM)"
parent: "book_1556559731"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N999544.html"
anchors: []
sha256: "0d0daab36d07d6684493b23570c03eb29a6dcead319c3796574b0beca5a303da"
---

DomainKeys Identified Mail (DKIM) is a method of digitally signing your email messages to allow authentication. To protect customers from spam, many ISPs check the domain key in an email to determine whether it is spam.

When you're sending email from your NetSuite production account, using your own domain key helps enhance your reputation as a legitimate marketer.

Important:

As of NetSuite 2024.1, DKIM setup has changed. NetSuite generates the necessary information (including the naming of the selector) for customers to add two DNS CNAME records at their domain provider's website. These two CNAME records let Oracle NetSuite manage the rotation of DKIM keys. The rotation of DKIM keys is an important security feature.

Only one CNAME record has a DKIM linked. This is an expected behavior.

To create your own domain keys:

-   A user with an Administrator role (or the Full level of the Set Up Company permission) must go to the Email Preferences page in NetSuite and set up your email domain on the **Email Domains (DKIM)** subtab.
    
-   A person with DNS experience must use the information generated in NetSuite and go to the website of your domain provider to add two CNAME records to DNS.
    

After completing the setup in NetSuite and adding CNAME records to DNS at your domain provider, your domain keys will authenticate email messages sent from NetSuite.

This section contains the following topics:

-   [Procedures to Set Up DKIM in Your Production Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1536091217.html)
    
    -   [Enter Email Domains in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163604950862.html)
        
        -   [Email Domains (DKIM) Details Column](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0124095724.html)
            
        -   [Email Domains (DKIM) Status Column](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0124093036.html)
            
    -   [Set Up CNAME Records in DNS](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163604971524.html)
        
-   [CNAMEs for Existing Email Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0126042246.html)
    
-   [Email Domains (DKIM) FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0125032558.html)
    
-   [More Information About DKIM](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163605022624.html)
    
    -   [FROM Headers in Email Can Be Rewritten](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1536091586.html)
        
    -   [Additional Sources of DKIM Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163605316433.html)
        

Note:

DKIM keys aren't copied to your non-production accounts. You're not required to set up DKIM keys in non-production accounts, although it's possible. Based on the email preferences set in sandbox or Release Preview accounts, email is typically sent only to a specified list of addresses, or to the logged-in user. For more information, see [Setting Preferences for Sandbox Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N334772.html) or [Setting Preferences for Release Preview Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1549916016.html#subsect_162376811938).

### Related Topics

-   [Opportunistic TLS and NetSuite Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163646559016.html)
-   [Size Limits for Emails and Attachments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7130136991.html)
-   [Email Blocklists and Spamlists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_156027670659.html)
-   [DMARC-Compliant Messaging in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1556559917.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
