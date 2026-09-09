---
id: "section_N2597878"
type: "section"
title: "Publishing Information to an Internal Site"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Tabs & Categories > Publishing Information to an Internal Site"
parent: "chapter_N2595349"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2597878.html"
anchors: ["bridgehead_N2597921", "procedure_N2597949", "bridgehead_N2598069", "procedure_N2598082"]
sha256: "1a7165d1507dc90e65cbeac311478fcf6edf36b5de4c44136c28ac6015d33a79"
---

With the Intranet feature, you can publish tabs and categories internally to specific roles, groups or individuals that have access to your NetSuite account.

For example, you can publish a tab internally to those who can access your account. Then, you can publish various categories, each with their own audience. Some employees, such as accountants, can have access to a category with information or announcements on payroll. Others, like support reps, access a category with information about cases or support policies.

## Publishing Tabs Internally {#bridgehead_N2597921}

Intranet tabs are different from center tabs. Intranet tabs let you publish information to an internal audience. Center tabs organize and give access to a set of page links and portlets in your NetSuite account.

For more information about center tabs, see [Creating Center Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2890512.html).

To publish tabs internally, an administrator must enable the Intranet feature at Setup > Company > Enable Features > Web Presence. Check the box next to Intranet, and click Save.

#### To create an intranet tab: {#procedure_N2597949}

1.  Go to _Setup > Intranet > Tabs > New_.
    
2.  Click **New Presentation** Tab.
    
3.  In the **Label** field, enter a name for the tab.
    
4.  Enter a **Greeting** and **Message** to show at the top of your site.
    
    The Greeting appears in bold text, and the Message shows under the greeting.
    
5.  Clear the **Display in Web Site** box to make sure this tab only shows in your NetSuite account.
    
6.  On the **Audience** subtab, select an audience for your intranet site:
    
    -   Check the **All** box to select all of a group, such as all customers, all vendors or all employees.
        
    -   If you check the **All Employees** box or select a name in the **Employees** field, an employee must have access to the Employee Center in order to view the tab.
        
    -   If you check **All Roles**, the tab is displayed for all roles, including customer, vendor and partner.
        
    
    Note:
    
    Press CTRL while selecting individual names or roles to highlight more than one.
    
7.  After you have selected everyone you want to see this tab, click **Save**.
    

Your new intranet tab appears in your account. To add information to your new tab, you must create categories and assign them to this tab.

You can also create a hosted tab for your intranet site by clearing the Display in Web Site box on the hosted tab record. For more information about audience permissions on hosted files, see [Audience Permissions for Hosted Sites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2598904.html). To learn how to create an intranet site, see [Creating an HTML Intranet Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2599141.html).

## Publishing Categories Internally {#bridgehead_N2598069}

You can create categories to publish information about your intranet page. Those you grant access to on the Audience subtab can see the categories published to the intranet tab when they log in.

#### To create a category for an intranet tab: {#procedure_N2598082}

1.  Go to _Setup > Intranet > Categories_.
    
2.  On the Site Category page, enter a name in the **Category** field.
    
3.  In the **Subcategory of** field, choose your intranet tab from the list.
    
4.  Clear the **Display in Web Site** box, and select the people who should be allowed to see the category on the Audience subtab. Each category can have its own audience so that each person will see information pertaining only to them.
    
    On the Audience subtab, you can give access to both static groups you manually create and dynamic groups that are based on search criteria. Both types of groups appear in the **Groups** list. If you use a dynamic group, for performance reasons, the tab's audience is a snapshot of the dynamic group members. The snapshot is updated twice a day.
    
5.  Click Save.
    

For more information about categories see, [Creating Site Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2596427.html).

### Related Topics

-   [Creating Website Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2595492.html)
-   [Creating Site Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2596427.html)
-   [Site Builder Tabs & Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2595349.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
