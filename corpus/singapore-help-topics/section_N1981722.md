---
id: "section_N1981722"
type: "section"
title: "Additional Setup Requirements for Singapore"
branch: "singapore-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Singapore Help Topics > Singapore Tax Topics for Accounts Without SuiteTax > Additional Setup Requirements for Singapore"
parent: "chapter_N1981261"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1981722.html"
anchors: []
sha256: "8bf8b4aac96dbad78f340398c41087f2a111979faa4b0339697df42e51ab488c"
---

If you have installed the NetSuite Tax Audit Files SuiteApp to generate the IRAS Audit File (IAF), you must complete the following setup steps:

Note:

For more information about what you must do to make the generated IAF compliant with IRAS requirements, see [Singapore Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1989169.html).

1.  Go to Setup > Accounting > Taxes > Set Up Taxes and set up tax preferences for Singapore.
    
2.  Enter your company's VAT/GST Registration No. and Unique Entity Number (UEN) on the company information (if you do not have a OneWorld account) or Singapore subsidiary record (if you have a OneWorld account). If you do not have a OneWorld account, go to _Setup > Company > Company Information_. If you have a OneWorld account, go to _Setup > Company > Subsidiaries_ and select the Singapore subsidiary.
    
3.  Go to _Go to Setup > Company > Setup Tasks > Auto-Generated Numbers_ and set up subsidiary numbering for transactions. For more information, see [Set Auto-Generated Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N252198.html).
    
4.  Go to _Go to Setup > Accounting > Preferences > Set Up Accounting_ and check the Use Account Numbers box. Also, make sure that each posting account has a unique account number in the Chart of Accounts setup. For more information, see [Chart of Account Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440268.html).
    
5.  Make sure the tax types and tax codes are set up as described in the following topics:
    
    -   [Singapore Tax Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983547.html)
        
    -   [Singapore Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983994.html)
        
6.  Fill in the UEN field on vendor records, partner records, and customer records. For details, see [Tracking the Unique Entity Number](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1986994.html).
    
7.  Mark the Reference No. field on the Vendor Bill, and the Check # field on Checks as required fields. To do so, an account administrator must complete the following configuration tasks:
    
    **Vendor Bills**
    
    1.  Create a custom vendor bill transaction form. Do one of the following to select the form to customize.
        
        -   Go to Transactions > Payables > Enter Bills and click Customize.
            
        -   Click Customize or Edit next to the form name at Customization > Transaction Forms. For example, click the Customize link of the Standard Vendor Bill.
            
    2.  Enter a name for the custom form. For example, Default Vendor Bill.
        
    3.  Check the Form is Preferred box to make this the default form that displays when a user creates a vendor bill.
        
    4.  On the Screen Fields subtab, in the Mandatory column, check the box next to Reference No. to mark the field as required on the custom form.
        
    5.  Click Save.
        
        ![An example of the screen fields subtab on a custom vendor bill transaction form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/CountrySpecificFeatures/SingaporeVendorBillCustomize.png)
    
    After saving the Custom Transaction Form, the custom Vendor Bill that you created now has the Reference No. field marked as required:
    
    ![Custom Vendor Bill with a Reference No. field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/CountrySpecificFeatures/SingaporeVendorBill.png)
    
    **Checks**
    
    1.  Create a custom check transaction form. Do one of the following to select the form to customize.
        
        -   Go to the Transactions > Bank > Write Checks and click Customize.
            
        -   Click Customize or Edit next to the form name at Customization > Transaction Forms. For example, click the Customize link of the Standard Check.
            
    2.  Enter a name for the custom form. For example, Default Check.
        
    3.  Check the Form is Preferred box o make this the default form that displays when a user creates a Write Check transaction.
        
    4.  On the Screen Fields subtab, in the Mandatory column, check the box next to Check # to mark the field as required on the custom form.
        
    5.  Click Save.
        
        ![An example of the screen fields subtab on a custom check transaction form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/CountrySpecificFeatures/SingaporeWriteCheckCustomize.png)
    
    After saving the Custom Transaction Form, the custom Check that you created now has the Check # field marked as required:
    
    ![Custom Check with a Check # field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/CountrySpecificFeatures/SingaporeWriteCheck.png)
    
    For details, see [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html) and [Configuring Fields or Screens](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856992.html).
    

### Related Topics

-   [Accounting for Goods and Services Tax - Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1987208.html)
-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Setting Up Tax Agencies as Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html)
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html)
-   [Setting Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1813668.html)
-   [Setting Tax Rounding Levels, Methods, and Precision Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1814149.html)
-   [Singapore Tax Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983547.html)
-   [Singapore Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983994.html)
-   [Additional Setup Requirements for Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1981722.html)
-   [Tracking the Unique Entity Number](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1986994.html)
-   [Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2073244.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
