---
id: "section_N2367472"
type: "section"
title: "Associating a Vendor With a Payroll Item"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Records > Vendor Record Configuration > Associating a Vendor With a Payroll Item"
parent: "article_161952107343"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2367472.html"
anchors: ["procedure_N2367763"]
sha256: "50aa6548b60222de8d50be0b76e1f0a60e51873b24e14bea6cca1c14138496af"
---

In NetSuite, you can set up payroll items and associate that item with a payroll vendor to simplify the withholding and payment of payroll liabilities. Examples of payroll liabilities are social service taxes such as Medicare, social security, unemployment, withholding of payroll taxes, health insurance payments, and 401(k) contributions. The following table provides a list of vendor records you may need to create and associate with payroll expenses and liabilities:

-   Internal Revenue Service for federal withholding and unemployment, as well as for company and employee contributions for Medicare and Social Security
    
-   State Department of Revenue for each state where employees live for state withholding, unemployment, and disability
    
-   City and local governmental authorities for any income taxes they are authorized to collect from their residents you employ
    
-   Group health/dental/vision insurance provider
    
-   Group life insurance provider
    
-   Group disability insurance provider (STD, LTD)
    
-   Retirement savings account manager (for example, pensions, 401(k)s, or IRAs)
    
-   Employee credit union for payroll-deduction savings plans
    
-   Flexible spending account manager
    
-   Labor union for dues
    
-   Charitable organizations for donations by deductions
    
-   Clerk of court or other collection agencies for garnishments
    

To associate a vendor with a payroll item, complete the following tasks:

-   Create or edit a vendor record. On the vendor record, assign that record to the Tax agency category and select the appropriate liability or expense account. For more information, see [Assigning a Vendor to the Tax Agency Category](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162151358618.html).
    
-   Create or edit a payroll item record. On the item record, select a payroll vendor as the Agency for that item.
    

#### To associate a vendor with a payroll item: {#procedure_N2367763}

1.  Go to _Lists > Employees > Payroll Items_.
    
2.  Check the **Show Inactives** box.
    
3.  Click **Edit** next to the payroll item you want to associate with a vendor.
    
    If you are creating a new payroll item, click **New** and select the type of item you want to create.
    
    Note:
    
    The Payroll feature must be enabled in your account to see payroll items in the list.
    
4.  On the payroll item record, select the appropriate vendor in the **Agency** field.
    
    Only vendors assigned to the **Tax** agency category appear in this list.
    
5.  If you are creating a new payroll item, enter information into the required fields for this item.
    
    Note:
    
    Set any limits in the **Limit** column on the Payroll Items page.
    
6.  Click **Save**.
    

NetSuite totals liabilities as you process payrolls. You can pay vendors associated with each liability as it becomes due. To do so, go to _Transactions > Bank > Pay Payroll Liabilities_.

### Related Topics

-   [Vendor Record Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161951406143.html)
-   [Enabling the Vendor Access Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161952527878.html)
-   [The Vendor Center Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2369118.html)
-   [Assigning a Role to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2363606.html)
-   [Giving Vendors Access to Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2364581.html)
-   [Vendor Records for 1099 Contractors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2364122.html)
-   [Vendor Credit Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2365918.html)
-   [Associating a Vendor With an Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2367376.html)
-   [Importing a Vendor Price List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2368077.html)
-   [Preferred Transaction Delivery on Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2368449.html)
-   [The Multiple Vendors Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2369578.html)
-   [Vendor Record Configuration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161952107343.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
