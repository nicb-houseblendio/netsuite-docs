---
id: "section_N295125"
type: "section"
title: "Mass Updating the Role Assigned to Customers"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Users & Roles > NetSuite Roles Overview > Mass Updating the Role Assigned to Customers"
parent: "section_N285436"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N295125.html"
anchors: ["procedure_N295140"]
sha256: "8cb9c17c3198b427f7ec58b784a999be42da43451b156b4cae51b85c0761fde0"
---

You can update the role assigned to your customers using a mass update. When you mass update customer roles, a change you indicate is made for many customer records at the same time, instead of changing the records one at a time.

For example, if you customize your Customer Center role and want to assign the new custom role to all of your customers, you can use the mass update to do so.

#### To mass update the customer role: {#procedure_N295140}

1.  Go to List > Mass Update > Mass Updates, expand Customer Support and Service and select Change Customer Role.
    
2.  In the **Title of Action** field, enter a name for this update.
    
3.  In the **Change Role** field, select the role you previously assigned that you now want to change.
    
4.  In the **to** field, select the role you want the update to assign in place of the role selected in the **Change Role** field.
    
    For example, in the **Change Role** field, you select Customer Center. In the **to** field, you select Customer Role Alpha, a custom role you created. When you run the mass update, selected customers are assigned the Customer Role Alpha role instead of the Customer Center role. These customers no longer have access to the Customer Center role.
    
5.  Define a filter or filters on the **Criteria** subtab to limit the customers whose role should be modified.
    
6.  Define display options for mass update results on the **Results** subtab.
    
7.  Define the users who can run the update on the **Audience** subtab, if available.
    
8.  If you have the Administrator role and you want to run the mass update on a recurring basis, set up this recurrence on the **Schedule** subtab. See [Scheduling a Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668529.html).
    
9.  View audited changes and actions respective to the update on the **Audit Trail** subtab.
    
10.  Click **Preview** to see which records the mass update will change, and review the Mass Update Preview page.
     
     -   To modify the mass update, click **Return to Criteria**, and repeat the previous steps as necessary.
         
     -   If your list has less than 1000 entries, an **Apply** column is shown. (If you want to show the **Apply** column, select search criteria that return results with less than 1000 entries. ) If any record listed should not be updated, clear the box in the **Apply** column.
         
11.  Choose one of the following options: **Return to Criteria**, **Perform Update**, or **Save**.
     
     you click **Perform Update**, you cannot stop or cancel the mass update, so proceed with caution!
     

For general information about mass updates, see [Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1103335211.html).

### Related Topics

-   [NetSuite Roles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285436.html)
-   [NetSuite Account Administration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4570420905.html)
-   [Separate Administration Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1491842937.html)
-   [Full Access Role (Deprecated)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1557254595.html)
-   [Permissions Requiring Two-Factor Authentication (2FA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515446005.html)
-   [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html)
-   [Changing Custom Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N289485.html)
-   [Inactivating Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N289968.html)
-   [Setting Default Forms for Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N290202.html)
-   [Restricting Accounts for Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N291349.html)
-   [Customizing the Customer Center Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N291685.html)
-   [Retail Clerk Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N291985.html)
-   [Showing Role Permission Differences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N292157.html)
-   [Use Searches to Audit Roles and Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460505281.html)
-   [Use Searches to Audit Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N292328.html)
-   [Use Searches to Audit Permissions By Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460505582.html)
-   [Mass Updating a Permission on Custom Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N293188.html)
-   [Standard Roles Permissions Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N295396.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
