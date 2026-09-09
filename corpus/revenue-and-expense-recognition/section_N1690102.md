---
id: "section_N1690102"
type: "section"
title: "Mass Updating Revenue Recognition Schedules"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Working with Revenue Recognition Schedules > Mass Updating Revenue Recognition Schedules"
parent: "section_N1689004"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1690102.html"
anchors: ["bridgehead_N1690121", "procedure_N1690137", "bridgehead_N1690207"]
sha256: "572ce24e6600d77941302f8c8a519a743c7264fb713091367f45634d117536fa"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For equivalent information about the current feature, see [Editing Revenue Recognition Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4369089832.html).

NetSuite provides two mass updates for revenue recognition schedules that you can run to update multiple records simultaneously. The Update is Recognized Flag mass update is available when the Revenue Recognition feature is enabled. The Create/Recreate Schedules on Sales Orders & Return Authorizations mass update is available when the Sales Order Revenue Forecasting feature is enabled.

## Update Is Recognized Flag {#bridgehead_N1690121}

The Is Recognized flag is used to identify revenue that has been recognized by a manual journal entry outside the revenue recognition journal entry process. You can update the Is Recognized field on many revenue recognition schedules simultaneously using a mass update. For all schedules that match the criteria set in the update form, the Is Recognized box is either checked or unchecked.

This mass update is designed to facilitate data migration when an opening balance is entered and revenue schedules span the period when the balance is entered. To avoid duplication, lines with posting dates prior to the period when the opening balance is entered should be marked as recognized.

#### To complete an Update Is Recognized Flag mass update: {#procedure_N1690137}

1.  Go to _Lists > Mass Update > Mass Updates_.
    
2.  Click **Rev Rec Schedules**.
    
3.  Click **Update Is Recognized Flag**.
    
4.  Complete the mass update form to set criteria, including selecting **Yes** or **No** in the **Is Recognized** field.
    
5.  Click **Preview** or **Save**.
    

## Create/Recreate Schedules on Sales Orders & Return Authorizations {#bridgehead_N1690207}

When you've enabled the Sales Order Revenue Forecasting feature, you can create and update recognition schedules for sales orders and return authorizations using mass update.

For example, you would like to create and update schedules for the last month on all sales orders and return authorizations. You can perform a mass update with the Date filter set for within the last month. When you submit the form, schedules are created for all appropriate lines on transactions.

If you also use the Project Management feature, this mass update enables you to create new schedules for existing projects or to update existing schedules for Sales Orders and return authorizations related to projects.

1.  Go to _Lists > Mass Update > Mass Updates_.
    
2.  Click **Create/Recreate Schedules on Sales Orders & Return Authorizations**.
    
3.  Complete the mass update form to set criteria.
    
4.  Click **Preview** or **Save**.
    

For more information about performing mass updates, read [Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1103335211.html).

### Related Topics

-   [Working with Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689004.html)
-   [Reviewing the Revenue Recognition Schedules List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689265.html)
-   [Viewing a Revenue Recognition Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689644.html)
-   [Editing a Revenue Recognition Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689901.html)
-   [Deleting a Revenue Recognition Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1690402.html)
-   [Cases When a Revenue Recognition Schedule May Not Be Created](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1691758.html)
-   [Creating a Revenue Recognition Schedule Dataset in SuiteAnalytics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0822023107.html)
-   [Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1103335211.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
