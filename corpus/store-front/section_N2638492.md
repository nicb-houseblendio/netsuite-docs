---
id: "section_N2638492"
type: "section"
title: "Importing Website Redirects"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > SEO & Analytics > Search Engine Optimization (SEO) > SEO and Redirects > Importing Website Redirects"
parent: "section_N2637891"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2638492.html"
anchors: ["bridgehead_N2638519", "bridgehead_N2638759", "procedure_N2638767"]
sha256: "d1ec0d2c22aa9edd75f9adccb30b721c530844c5abf4c0aaf189175324dbbe2f"
---

Besides [Setting Up a URL Redirect](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2638072.html) individually on the Redirect record page, you can use the website redirects import assistant to add and update URL redirects in bulk from a CSV file. You can import up to 100,000 URL redirects at one time.

This import assistant is available at Commerce > Hosting > Redirects > Import, when the Web Site and Host HTML Files features are enabled. You'll need the Set Up Web Site permission.

## CSV Template File for URL Redirects {#bridgehead_N2638519}

The website redirects import assistant includes a link to a CSV template file. Populate your CSV file with the following fields for each redirect record:

| **Field** | **Notes** |
| --- | --- |
| Domain Name | 
Must match the name of an existing domain.

You need to set up domains in NetSuite before importing URL redirects. See [Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2478982.html).

Maximum field size= 80 |
| Redirect From URL | Must be a relative URL that is also a descriptive URL. Maximum field size=4000 |
| Redirect To URL | Can be any of the following:

-   a relative URL that points to an HTML page on your NetSuite site
-   a descriptive URL that points to a tab, category, or item detail page
-   an absolute URL that points to another site

Maximum field size=4000 |

For example, to redirect visitors from /old-products to /featured-products on www.example.com, use the following values:

-   Domain Name: www.example.com
    
-   Redirect From URL: /old-products
    
-   Redirect To URL: /featured-products
    

Relative URLs include the path but not the domain. Use a leading slash.

## Using the Website Redirects Import Assistant {#bridgehead_N2638759}

#### To import URL redirects from a CSV file: {#procedure_N2638767}

1.  Go to _Commerce > Hosting > Redirects > Import_.
    
2.  Click the **Redirect Template File** link.
    
3.  Save the CSV file and populate it with your data, following the guidelines provided.
    
4.  In the Import Assistant, click **Select**, and then browse to your CSV file. Click **Next**.
    
    The second page of the Import Assistant shows how the fields in your file are mapped to NetSuite fields. This mapping is automated and you should not have to change it.
    
    ![Import assistant mapping example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Commerce/StoreFront/SEOandAnalytics/RedirectMapping.png)
5.  Click **Run**.
    

During the import, the system attempts to match the **Domain Name** and **Redirect From URL** values to existing redirect records.

-   If a match is found, the import updates the existing redirect record with the Redirect To URL value.
    
-   If no match is found, the import adds a new redirect record.
    

You can use the import Job Status page to review the progress of your import. Note that the count of redirect records successfully imported to NetSuite includes only values for Redirect From URL in the CSV file used for import.

### Related Topics

-   [Updating Redirect Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2638305.html)
-   [Delete Web Site Redirects Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2638981.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
