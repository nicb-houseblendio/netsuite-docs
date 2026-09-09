---
id: "chapter_N2999459"
type: "chapter"
title: "Creating Script Parameters"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > Creating Script Parameters (Custom Fields) > Creating Script Parameters"
parent: "part_1542289448"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999459.html"
anchors: []
sha256: "7ec38bdba6d5886214f921762254285b754bdcab02432eb504798089c90c9a83"
---

Use the following steps to create script parameters. If you're unsure how to create a script record, see [Creating a Script Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489062315.html).

#### To create a script parameter:

1.  Go to _Customization > Scripting > Scripts_.
    
2.  Beside the script you want to add a parameter to, click **Edit**.
    
3.  Click the **Parameters** subtab, and click **New Parameter**.
    
4.  In the **Label** field, type the name of the parameter (custom field) as it will appear in the UI after the script is deployed.
    
5.  In the **ID** field, type a custom ID for the script parameter.
    
    Use lowercase and no spaces for script parameter IDs. They also cannot exceed 30 characters.
    
    You can leave the ID field blank to use a system-generated ID. However, it is a best practice to create your own custom ID for script parameters. This helps avoid naming conflicts if you add your script to a SuiteCloud project later.
    
6.  In the **Type** field, select the type of the script parameter (for example, Hyperlink, Date, Free-Form Text, or Check Box).
    
    For more information about field types, see [Field Type Descriptions for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2842731.html).
    
7.  (Optional) If the parameter type is List/Record, in the **List/Record** field, specify the list or record.
    
    If you define a saved search as a List/Record script parameter, only saved searches that are public will appear in the List/Record field. For more information about working with searches using SuiteScript, see [N/search Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345764122.html).
    
8.  In the **Preference** field, select the set of preferences that you want to use for the parameter.
    
    The parameter's default value is based on the values set on either the General Preferences page (for a field value of Company), Set Preferences page (for a field value of User), or the portlet setup page (for a field value of Portlet), depending on the field value. If you do not specify a preference, the parameter is considered to be a deployment script parameter, and its value is defined on the script deployment record.
    
    For more information, see [Script Parameter Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999849.html).
    
9.  (Optional) Use the **Display**, **Validation & Defaulting**, **Sourcing & Filtering**, **Access**, and **Translation** tabs to define additional values for the parameter.
    
    For information about defining these values, see the following help topics:
    
    -   [Setting Display Options for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830238.html)
        
    -   [Setting Validation and Defaulting Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830711.html)
        
    -   [Setting Sourcing Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2839623.html)
        
    -   [Setting Filtering Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2840153.html)
        
    -   [Restricting Access to Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2841053.html)
        
    -   [Adding Translations for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4308565496.html)
        
10.  Click **Save** to save the parameter.
     
11.  On the script record, click **Save** to save the script record.
     

### Related Topics

-   [Creating Script Parameters Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999300.html)
-   [Referencing Script Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999784.html)
-   [Script Parameter Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999849.html)
-   [Setting Script Parameter Preferences Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3000000.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
