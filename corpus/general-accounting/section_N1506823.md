---
id: "section_N1506823"
type: "section"
title: "Creating Budget Categories for Local Subsidiary Budgeting"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Budgets > Budgets in NetSuite > Subsidiary Budgets in OneWorld > Creating Budget Categories for Local Subsidiary Budgeting"
parent: "section_N1506361"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506823.html"
anchors: ["procedure_N1506848"]
sha256: "c23ad0e8e288e7e3313c5d3a127b5fe7cb2b7e2172ca28d98f2d5784d88b86bc"
---

When the Multiple Budgets feature is enabled, you can use budget category values on budget records to categorize types of budgets. In NetSuite OneWorld, budget category values are used to indicate whether budgeting is done at the local subsidiary level in local currency or globally using the root subsidiary's currency. Each budget category is associated with a budget category type of local or global.

You're required to use budget categories only if you have multiple budgets. For an overview, see [Multiple Budgets and Budget Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506174.html).

You should create budget categories before you create additional budgets.

#### To create a budget category: {#procedure_N1506848}

1.  Go to _Setup > Accounting > Accounting Lists > New_.
    
2.  On the Add to Accounting Lists page, click the link to **Budget Category**.
    
3.  Enter a descriptive name. This name appears in lists.
    
4.  Check the **Global** box to indicate that budgets assigned this budget category have a type of global, and are defined in the base currency of the root parent subsidiary.
    
    If this box is not checked, this budget has a budget category type of local, indicating that budgets assigned this category are defined in the base currency of the individual subsidiary.
    
    To develop and test budget alternatives, you can create multiple global and local budgets for each subsidiary.
    
    For information about working with budget category types in reports, see [Subsidiary Budgets in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506361.html).
    
5.  To make this budget category available for immediate use, make sure the **Inactive** box is clear.
    
6.  Click **Save**.
    

### Related Topics

-   [Subsidiary Budgets in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506361.html)
-   [Subsidiary Budgeting Scenario](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506662.html)
-   [Setting Up a Subsidiary Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1507295.html)
-   [Guidelines for Copying a Subsidiary Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1507638.html)
-   [CSV Import for Subsidiary Budgets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1508163.html)
-   [Budget Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1508302.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
