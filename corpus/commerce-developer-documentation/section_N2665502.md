---
id: "section_N2665502"
type: "section"
title: "The Base URL"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Item Search API > The Base URL"
parent: "chapter_N2665337"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2665502.html"
anchors: ["subsect_163948681771"]
sha256: "6a4289ddfc7771a61e74a32c5d06abec2ead7c79b3a95f21c7812e5ebb222476"
---

The Item Search API is typically consumed by an AJAX client. You can use a client-side JavaScript framework like jQuery to send an HTTP request to the API and get the JSON response back. The URL is accessible by any client that supports HTTP and JSON. You can retrieve results for a particular item search by sending an HTTP GET request.

The Item Search API base URL has the following format:

`http://www.mywebstore.com/api/items`

The components of the base URL are described here:

-   **Custom Domain** - A unique URL is required, which must be a custom domain. For example, `www.mywebstore.com` is a custom domain.
    
-   **Items** - This API is designed to query item records in your NetSuite account. Note that `/api/items` in the URL is part of the path and it is required. You cannot assign a value to it.
    
-   **Parameters** - You can use parameters defined by NetSuite along with values from your account. You can use multiple parameters in an Item Search API request by separating them with an ampersand (&). Parameters are typically name-value pairs, such as `fieldset=details`. For more information, see [Item Search API Input Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2665676.html).
    

Note:

JSONP (JSON with padding) wraps the JSON response from API requests in a JavaScript variable that can be included in a script tag to enable cross-domain AJAX requests. Web developers can use callback as the input parameter as described in Callback Function, and then create the variable name. For more information about the jQuery API, see [api.jquery.com/jQuery.getJSON/](http://api.jquery.com/jQuery.getJSON/).

## Cacheable and Personalized Endpoints {#subsect_163948681771}

The Item Search API has two additional endpoints:

-   `/cacheable/items` - responses are cached. This endpoint works in the same way as the `/items` endpoint.
    
-   `/personalized/items` - responses are never cached. This endpoint retrieves personalized item information that is specific to a customer.
    

Since the 2021.2 release of SuiteCommerce and SuiteCommerce Advanced (SCA), cacheable or personalized API endpoints are automatically used depending on whether a user is logged in to your Commerce website and whether the personalized endpoint configuration option has been enabled.

Example: Personalized API endpoints are used if the user is logged in and you have enabled the personalized endpoint configuration option.

If the user is not logged in, any of the following URLs can be used as both endpoints work the same way:

-   `http://www.mywebstore.com/api/items`
    
-   `http://www.mywebstore.com/api/cacheable/items`
    

The URL `http://www.mywebstore.com/api/items` can be used for SCA versions 2021.1 and earlier.

Personalized API endpoints are enabled by default. However, you can verify that they are enabled by checking the SuiteCommerce Configuration.

Note:

To ensure that logged-in users receive personalized catalog views that are not cached for other users, you should enable personalized API endpoints.

#### To verify that the personalized API endpoints are enabled:

1.  In NetSuite, go to Commerce > Websites > Configuration.
    
2.  Select your website and domain and click **Configure**.
    
3.  Go to the **Shopping Catalog** tab.
    
4.  Check the **Enable New Search API Endpoints** box.
    
5.  Click **Save**.
    

For information about the configurable property, see [Enable Personalized Search API Endpoints](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4667037093.html#subsect_162617387984).

### Related Topics

-   [Item Search API](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2665337.html)
-   [Items Available to the Item Search API](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1520340184.html)
-   [Item Search API Input Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2665676.html)
-   [Item Search API Output Response](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509454056.html)
-   [Sample Item Search Query and Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2667130.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
