---
id: "chapter_N1016228"
type: "chapter"
title: "Promotional URLs"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Promotional URLs"
parent: "book_N973201"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1016228.html"
anchors: ["procedure_N1016309", "procedure_4480583521"]
sha256: "da337cf50f16cdd4fd78a2b9b1c379ee48faaa9ede19bb90bb5798750e98af67"
---

Promotional URLs are short, descriptive links that take users to online forms, categories, or items in your website.

For example, the URL NetSuite assigns to the Information tab of the Wolfe Electronics website is http:// www.wolfeelectronics.com/app/site/site.nl/site.ACCT00000/mode.items/sc.5/.f. By creating a promotional URL, Wolfe can promote this page to customers as http://www.wolfeelectronics.com/information. When customers enter the promotional URL, they are taken to the Information tab of Wolfe's site.

If you include a promotional code in the URL, NetSuite applies discounts associated with the promotion to any order placed during that site visit.

Before you set up promotional URLs, you must set up your own domain through a domain registrar. For more information, see [Domain Setup Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1521794882.html#section_1521797541).

#### To create a promotional URL: {#procedure_N1016309}

1.  Go to _Setup > Marketing > Setup Tasks > Promotional URLs_.
    
    The URL you create appears in the **Composite URL** field.
    
2.  In the **Name** field, enter the word or phrase you want customers to enter as the URL.
    
    This word or phrase appends the URL in the **Base URL** field.
    
3.  In the **Description** field, enter a short message describing this promotional URL.
    
4.  In the **Page Type** list, select a type of page to link to from the following list:
    
    -   File Cabinet Item
        
    -   Hosted Web Page
        
    -   Knowledge Base Topic
        
    -   Online Case Form
        
    -   Online Customer Form
        
    -   Web Site Category
        
    -   Web Site Information Item
        
    -   Web Site Item
        
    -   Web Site Tab
        
5.  In the **Page** list, select the page you want to link to.
    
6.  In the **Additional Parameters** field, enter the descriptive information you want to pass through the URL.
    
    -   Enter up to 40 characters in this field.
        
    -   Enter parameters in the following format: ID=value.
        
        -   In place of ID, enter the ID listed in the table below for the field you want to enter information into.
            
        -   In place of value, enter the value you want to automatically appear in this field.
            
        -   String parameters together with ? and & symbols. The first parameter in a URL should begin with a ?. Subsequent parameters should begin with &. For example, category=individual&partner=Hill's Fine Jewelry.
            
7.  Click **Save**.
    

| **Field** | **ID** |
| --- | --- |
| Company Name | companyname |
| Address Line 1 | address1 |
| Address Line 2 | address2 |
| City | city |
| State | state |
| Zip Code | zipcode |
| Country | country |
| Contact First Name | firstname |
| Contact Middle Name | middlename |
| Contact Last Name | lastname |
| Currency | currency \*Use currency abbreviation, such as USD. |
| Customer Category | category |
| E-mail | email |
| Login Password | password |
| Partner/Partner Code | partner |
| Phone Number | phone |
| Lead Source | leadsource |
| Promotion | promocode |
| Unsubscribe to E-mail Campaigns | unsubscribe |
| Web Address | url |

Customers can now access your web pages with this promotional URL. If customers use a promotional URL that's different from your site's domain name, the URL might change to the default display URL.

#### NetSuite determines the domain in the URL using the following rules: {#procedure_4480583521}

1.  The first domain hosted as a Promotional URL at _Commerce > Hosting > Domains_.
    
2.  The domain used in the web store primary site URL.
    
3.  The first domain name that begins with www and is hosted as a hosted web page.
    
4.  If there is no hosted web page domain that begins with www, NetSuite uses the first domain hosted as a hosted web page.
    
5.  If 1 - 4 do not apply, NetSuite uses the first domain name in the list on the Domains page that begins with www.
    

### Related Topics

-   [Email Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N993117.html)
-   [Optimizing Email Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N993465.html)
-   [Campaign Email Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N996559.html)
-   [DomainKeys Identified Mail (DKIM)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N999544.html)
-   [How is bounced campaign email handled?](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3898540.html#question_N3899955)
-   [Mail Merge vs. Email Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N991127.html)
-   [Creating a Campaign Email Address Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1000747.html)
-   [Campaign Subscription Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N996344.html)
-   [Email Marketing Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1001310.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
