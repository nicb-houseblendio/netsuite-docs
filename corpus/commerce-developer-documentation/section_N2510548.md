---
id: "section_N2510548"
type: "section"
title: "PageGenerator Methods"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > Shopping Objects > PageGenerator Methods"
parent: "section_N2496577"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html"
anchors: ["bridgehead_4482716131", "bridgehead_3995735380", "bridgehead_4482716368", "bridgehead_3995736416", "bridgehead_4482716580", "bridgehead_3995736860", "bridgehead_4482716776", "bridgehead_3995737355", "bridgehead_4482716981", "bridgehead_3995738267", "bridgehead_4482717181", "bridgehead_3995738780", "bridgehead_4482717398", "bridgehead_3995739060", "bridgehead_4482717610", "bridgehead_3995739485", "bridgehead_4482717838", "bridgehead_3995739798", "bridgehead_4482718208", "bridgehead_3995740279", "bridgehead_4482718420", "bridgehead_3995741003", "bridgehead_4482718755", "bridgehead_3995742449", "bridgehead_4482719060", "bridgehead_3995749797"]
sha256: "586093501146a7c8d0ac05e9e01991d56480ebd2ee1f4051ba9df54d69b422b5"
---

Methods on the pageGenerator object are used to generate a web store page.

The following PageGenerator methods are available:

-   [addBreadCrumb(label, url)](#bridgehead_4482716131)
    
-   [addHeadHtml(html)](#bridgehead_4482716368)
    
-   [addStylesheetHtml(html)](#bridgehead_4482716580)
    
-   [addTab(id, label, url)](#bridgehead_4482716776)
    
-   [addToPageInitScript(scriptLines)](#bridgehead_4482716981)
    
-   [removeBreadCrumbs()](#bridgehead_4482717181)
    
-   [removeTab(id)](#bridgehead_4482717398)
    
-   [removeTabs()](#bridgehead_4482717610)
    
-   [setDocTypeHtml(html)](#bridgehead_4482717838)
    
-   [setMetaTagHtml(html)](#bridgehead_4482718208)
    
-   [setPageTitle(title)](#bridgehead_4482718420)
    
-   [setSelectedTab(id)](#bridgehead_4482718755)
    
-   [showTabNavigation(show)](#bridgehead_4482719060)
    

## addBreadCrumb(label, url) {#bridgehead_4482716131}

Adds a bread crumb to the end of the existing bread crumb trail.

## Parameters {#bridgehead_3995735380}

-   `label` \[required\] {string} - text displayed for the bread crumb
    
-   `url` \[required\] {string} - URL to which the bread crumb links
    

**Back to** [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## addHeadHtml(html) {#bridgehead_4482716368}

Adds the specified HTML to the top of the page's <head> section, before the stylesheet HTML.

## Parameters {#bridgehead_3995736416}

-   `html` \[required\] {string} - HTML content
    

**Back to** [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## addStylesheetHtml(html) {#bridgehead_4482716580}

Adds the specified HTML to the top of the page's <head> section, after the stylesheet HTML

## Parameters {#bridgehead_3995736860}

-   `html` \[required\] {string} - HTML content
    

**Back to** [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## addTab(id, label, url) {#bridgehead_4482716776}

Adds a tab to the right of current tabs on the page.

## Parameters {#bridgehead_3995737355}

-   `id` \[required\] {string} - unique string id for the tab
    
-   `label` \[required\] {string} - label displayed within the tab
    
-   `url` \[required\] {string} - URL to which the tab links
    

**Back to** [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## addToPageInitScript(scriptLines) {#bridgehead_4482716981}

Adds lines of JavaScript to the page's initialization script.

## Parameters {#bridgehead_3995738267}

-   `scriptLines` \[required\] {string}
    

**Back to** [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## removeBreadCrumbs() {#bridgehead_4482717181}

Removes all bread crumbs from the page.

## Parameters {#bridgehead_3995738780}

No parameters to set.

**Back to** [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## removeTab(id) {#bridgehead_4482717398}

Removes a specified tab from the page.

## Parameters {#bridgehead_3995739060}

-   `id` \[required\] {string} - unique string id for the tab
    

**Back to** [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## removeTabs() {#bridgehead_4482717610}

Removes all tabs from the page.

## Parameters {#bridgehead_3995739485}

No parameters to set.

**Back to** [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## setDocTypeHtml(html) {#bridgehead_4482717838}

Establishes HTML for the page `<doctype>` tag.

## Parameters {#bridgehead_3995739798}

-   `html` \[required\] {string} - HTML content
    

**Back to** [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## setMetaTagHtml(html) {#bridgehead_4482718208}

Establishes HTML for the page's `<meta>` tags.

## Parameters {#bridgehead_3995740279}

-   `html` \[required\] {string} - HTML content
    

**Back to** [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## setPageTitle(title) {#bridgehead_4482718420}

Establishes a title for the page.

## Parameters {#bridgehead_3995741003}

-   `title` \[required\] {string} - title text
    

**Back to** [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## setSelectedTab(id) {#bridgehead_4482718755}

Causes the specified tab to be displayed as the currently active tab.

## Parameters {#bridgehead_3995742449}

-   `id` \[required\] {string} - unique string id for the tab
    

**Back to** [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html) | **Back to** [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

## showTabNavigation(show) {#bridgehead_4482719060}

Indicates whether tab navigation should be shown or hidden.

## Parameters {#bridgehead_3995749797}

-   `show` \[required\] {boolean} - true to display navigation, false to hide it
    

### Related Topics:

-   [Input Parameters/Return Values for Shopping Object Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497278.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
