---
id: "section_N918520"
type: "section"
title: "Entering Workplace Records for Payroll"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Setup > Entering Workplace Records for Payroll"
parent: "chapter_N917379"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N918520.html"
anchors: ["procedure_N918559", "subsect_1556723230"]
sha256: "321d6e5d13ccac5700c2cdfc0eb2700fc5b1426cd249331f0820be2b83b121fc"
---

To use SuitePeople U.S. Payroll, you must set up a workplace record for every location with a tax ID and paid employees. NetSuite uses workplace records to identify which taxes you'll need to withhold and pay. Every employee in a payroll batch must have a designated workplace.

Note:

The workplace address can be used along with a home address.

#### To create workplace records: {#procedure_N918559}

1.  Go to _Lists > Employees > Workplaces > New_.
    
    Workplaces also are listed in the **Main Office** field on the **Preferences** tab of the Set Up Payroll page. If you're new to Payroll, you must create a workplace record for your main office.
    
2.  In the **Name** field, enter a name for the workplace.
    
    This name appears on forms and reports where you need to choose a workplace.
    
    For example, you could name one location Georgia Warehouse and another California Headquarters.
    
3.  If the workplace is part of another, select the parent workplace from the **Subworkplace of** field.
    
4.  To add the workplace address, click **Edit** next to the **Address** field. Complete the fields in the address, including the following:
    
    1.  In the **Attention** field, enter the person at this address who should be notified of receipt of documents or goods.
        
    2.  In the **Addressee** field, enter the company name for this workplace as it should appear on labels and transactions.
        
        This name appears under the name you enter in the **Attention** field.
        
    3.  Enter the phone number for this workplace as you want it to appear on forms.
        
    4.  Enter the address for this workplace.
        
        You must include the full street address, state, and zip code for each workplace record. The Payroll feature uses this address to calculate taxes.
        
    5.  Click **OK**.
        
5.  Click **Save**.
    

If the workplace is in Alaska, you can edit it after saving to add a geographic code. For more information, see [Adding Geographic Codes to Alaska Workplaces](#subsect_1556723230).

After you create the workplace record, you can select the new workplace from the **Workplace** field on the Payroll subtab of the employee record.

Note:

You cannot delete a workplace if it is referenced in any employee record. If you don't want a workplace to appear in lists, check the **Workplace is Inactive** box.

## Adding Geographic Codes to Alaska Workplaces {#subsect_1556723230}

If a workplace is in Alaska, you must enter a geographic code on the workplace record.

Before you can add geographic codes to Alaska workplaces, you must install the Payroll Compliance SuiteApp.

-   **Bundle Name**: Payroll Compliance
    
-   **Bundle ID**: 202280
    

To learn how to install a SuiteApp, see [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html).

#### To add a geographic code to an Alaska workplace:

1.  Go to _Lists > Employees > Workplaces_.
    
2.  Beside an Alaska workplace, click **Edit**.
    
3.  In the **Geographic Code** field, enter the two-digit geographic code. For more information about geographic codes, see [live.laborstats.alaska.gov/erg/geocodes.cfm](http://live.laborstats.alaska.gov/erg/geocodes.cfm).
    
4.  Click **Save**.
    

### Related Topics

-   [Enabling Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N917966.html)
-   [Entering Company Information for Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N918232.html)
-   [Updating Payroll Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N930407.html)
-   [Payroll Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N920073.html)
-   [Retirement Plan Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162558111263.html)
-   [Payroll Items Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N930985.html)
-   [Payroll Setup for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921632.html)
-   [Running Test Payroll Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N944846.html)
-   [Setting up Year-To-Date Information From Your Previous Payroll System](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N944369.html)
-   [Entering a Payroll Start Date](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N945629.html)
-   [Payroll Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N917379.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
