---
id: "section_N2880594"
type: "section"
title: "Applying Role-Based Restrictions to Custom Records"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Records Overview > Creating Custom Record Types > Applying Role-Based Restrictions to Custom Records"
parent: "section_N2876492"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880594.html"
anchors: []
sha256: "f972d7a476493240c8fc5ebf7a70d01ba1cef1698a7cc27e4c55ec2ea218756d"
---

On a role record, you can restrict the access of users with that role to standard records, based on these records' values for department, class, location, employee, and subsidiary (OneWorld) fields. For example, you could set an employee-based restriction for the Sales Manager role so that those users see only records where they or their subordinates are the sales rep.

For details about setting these restrictions, see the following topics.

-   [Setting Employee Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4637690919.html)
    
-   [Setting Department, Class, and Location Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4637695352.html)
    
-   [Restricting Role Access to Subsidiaries (OneWorld Only)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N286421.html)
    
-   [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html)
    

You can apply the restrictions set on role records for a particular category (department, class, location, employee, or subsidiary) to a custom record, by checking the Apply Role Restrictions box for a list/record custom field that stores values in one of these categories. For example, if you check this box for an Employee list/record custom field, the employee-based restriction set on the Sales Manager role record is applied to this custom record. Those users see only custom records where they or their subordinates are the value for the custom field.

When a custom record has a field that permits restrictions, and the Apply Role Restrictions box is checked, empty fields aren't included when the restrictions are applied. With role restrictions enabled for a custom record, you can't view or edit records where the role-related field is empty. For example, if your user role is restricted to Subsidiary A, and a custom record is created that does not specify a subsidiary, your view is restricted to Subsidiary A. You'll only see records with Subsidiary A selected, and you won't see any records with blank subsidiary fields.

Choose the next step, based on your needs:

-   [Applying Role-Based Access Restrictions to Custom Records if the Class, Department, Location, Employee, or Subsidiary Field Does Not Yet Exist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_161955076550.html).
    
-   [Applying Role-Based Access Restrictions to a Custom Record if the Field Already Exists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_161955113705.html).
    

### Related Topics

-   [Applying Role-Based Access Restrictions to Custom Records if the Class, Department, Location, Employee, or Subsidiary Field Does Not Yet Exist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_161955076550.html)
-   [Applying Role-Based Access Restrictions to a Custom Record if the Field Already Exists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_161955113705.html)
-   [Creating Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2876492.html)
-   [Creating a New Custom Record Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501860307.html)
-   [Entering Name and Display Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501860247.html)
-   [Specifying Permission and UI Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501860092.html)
-   [Configuring File and Child Record Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501859968.html)
-   [Defining Search and Edit Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501859705.html)
-   [Adding Fields to Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2878340.html)
-   [Limiting Search Access to Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880332.html)
-   [Adding Subtabs to a Custom Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2877748.html)
-   [Choosing an Icon for a Custom Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2881257.html)
-   [Numbering Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2878042.html)
-   [Adding Custom Forms for a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2878636.html)
-   [Online Custom Record Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2882522.html)
-   [Setting Up a Permissions List for a Custom Record Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2879931.html)
-   [Creating Links to Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880942.html)
-   [Adding Translations for Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2882154.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
