---
id: "section_N1797005"
type: "section"
title: "Setting Tax Codes or Tax Schedules on Item Records"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Enabling and Setting Up Taxation Features > Setting Tax Codes or Tax Schedules on Item Records"
parent: "chapter_N1794679"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797005.html"
anchors: ["procedure_N1797017"]
sha256: "bd4e761e8c48c0597d97b488b75c94125036f705351371445b09ca2160f69fb5"
---

On an item record, you must set a default tax code or tax schedule to be applied to that item. In U.S. editions without Advanced Taxes, you can only set an item to be either taxable or not taxable.

#### To set tax items on item records: {#procedure_N1797017}

1.  Create an item record by going to Lists > Accounting >Items > New.
    
2.  Click the item type of the item you want to create.
    
3.  On the **Accounting** subtab of the item record, select the appropriate tax code or tax schedule:
    
    -   For accounts without Advanced Taxes, select a tax code.
        
    -   For accounts that have Advanced Taxes enabled, select a tax schedule.
        

Warning:

When you inactivate a tax control account, any tax codes associated with it will no longer be available for selection when you create or edit a transaction record. Also, any existing default tax codes and tax schedules associated with the inactivated tax control account will be invalidated. Be sure to change the default tax codes and tax schedules on the affected item records. Alternatively, you can reactivate the tax control account. For more information, see [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html).

### Related Topics

-   [Tax Setup Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1795438.html)
-   [Enabling Taxation Features in Accounts Without Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1795648.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
