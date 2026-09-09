---
id: "section_N279420"
type: "section"
title: "Currency for Multiple Subsidiary Search Results"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Consolidated Reporting in OneWorld > Currency for Multiple Subsidiary Search Results"
parent: "section_N278654"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N279420.html"
anchors: []
sha256: "541e941b132e0cb9e36dc4c2ae7c3e6445a00cdafc840d579111ac57aec219c7"
---

When you view search results for multiple subsidiaries, results are converted (consolidated exchange rates) into the currency of the lowest common parent (LCP).

For example, a business hierarchy looks like this:

![Diagram of subsidiary context specific to currencies.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/NetSuiteOneWorld/UnderstandingSubsidiariesContextForReports.png)

For example, a user with access to the Singapore and Japan subsidiaries runs a search. The search results display all currency amounts in UK pounds because Wolfe UK is the LCP for these subsidiaries. If the user had access to Japan and Germany, currency amounts would display in US dollars.

You can limit the data returned to a single subsidiary. Go to _Home > Set Preferences_ > Restrict View subtab. See [Restrict Your Subsidiary View](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278473.html).

Tip:

You can select the type of exchange rate applied to and advanced search or saved search of transactions. Choose the Consolidated Exchange Rate option for search results. See [Consolidated Exchange Rate Types for Transaction Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1409190.html).

### Related Topics

-   [Subsidiary Context for Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278946.html)
-   [Consolidated Reporting in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278654.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
