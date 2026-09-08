---
id: "section_N324233"
type: "section"
title: "Login Audit Trail Overview"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Users & Roles > NetSuite Users Overview > Login Audit Trail Overview"
parent: "section_N321756"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N324233.html"
anchors: ["bridgehead_3746130433"]
sha256: "dd3a271c46b296ed591b2d797941883fd76d3d8fc329ab09901ed842fc02c6de"
---

The Login Audit Trail is a specialized search that helps keep track of account users, when they have logged in, and from where. It is available at _Setup > Users/Roles > View Login Audit Trail_.

The Login Audit Trail captures and records the IP address at the beginning of the user's session. It does not capture changes in IP addresses that might occur during a session, such as when a user connects to a Virtual Private Network (VPN) during an active session. If the user logs out of NetSuite, then logs back in when the VPN is still open, the IP address of the VPN will be captured for that session.

Note:

Oracle NetSuite does not support traffic that is routed through a split-tunnel Virtual Private Network (VPN) to control user access to NetSuite. For more information, see [VPN Configuration for User Access to NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161609571818.html).

This search returns a list of login activity, that can include each session listed by date and time of initial login, the user's name, and the IP address from which the user logged in. When you drill down on individual login entries, you view a list of the transactions completed during the user's session. If no data appears, then the user did not complete any transactions during the period you are viewing.

Note:

You can also find the Login Audit Trail search from general search task links, like _Reports > New Search_, and _Reports > Saved Searches > All Saved Searches > New_.

## Login Audit Trail Search Capabilities {#bridgehead_3746130433}

The Login Audit Trail offers the same capabilities as other NetSuite searches, including:

-   Simple search mode, where you can select from a limited set of filters, including IP address, user name, date range, and role.
    
-   Advanced search mode, with more options, including filtering by formulas and join fields, display of formula and join fields as results, and sorting and grouping of results. Available join fields include Role, Employee, and in some cases, Customer, Partner, and Vendor fields.
    
-   Saved searches that you can define and run repeatedly. Saved searches offer all advanced search options, and more, including defining audiences and sending emails of search results.
    

When you open the Login Audit Trail Search page it displays in the mode last used, initially simple search.

For instructions for using the Login Audit Trail, see the following:

-   [Defining a Simple Login Audit Trail Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1548084502.html)
    
-   [Defining an Advanced Login Audit Trail Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1548084729.html)
    

### Related Topics

-   [NetSuite Users Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N321756.html)
-   [Employee Users](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N322041.html)
-   [Vendor Users](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N322273.html)
-   [Partner Users](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N322424.html)
-   [Customer Users](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N322570.html)
-   [Giving Customers Access](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N322750.html)
-   [Changing a User's NetSuite Password](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N323774.html)
-   [Viewing Your NetSuite Users List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N324056.html)
-   [Inactivating Users](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1525773325.html)
-   [Restricting an Individual User View](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N324888.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
