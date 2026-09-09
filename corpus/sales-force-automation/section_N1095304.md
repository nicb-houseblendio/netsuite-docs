---
id: "section_N1095304"
type: "section"
title: "Mapping Custom Lead Fields"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Record Management > Lead Management > Lead Conversion > Lead Conversion Using the Lead Conversion Feature > Mapping Custom Lead Fields"
parent: "bridgehead_N1086741"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1095304.html"
anchors: ["procedure_N1095329"]
sha256: "da466cc017f2843ab785544a4b8e1f37a925e5aa2fa5d130fab16645c2acab0b"
---

If the Lead Conversion feature is enabled in your account, you can map custom fields on your lead records to custom fields on contact, opportunity, and task records. When you convert a lead, the values of these custom fields are automatically carried over. However, you can map only fields that are of the same type. For example, you can't map a text field to a list or record field. For information about creating custom fields for lead records, see [Creating Custom Entity Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2827562.html).

When you map a custom lead field, only the contact, opportunity, and task custom fields of the same type appear for mapping. Fields of other types don't appear.

#### To map lead custom fields: {#procedure_N1095329}

1.  Go to _Setup > Sales > Lead Conversion Mapping_.
    
2.  To automatically add the following types of custom fields, click **Auto Map Fields**:
    
    -   Custom entity fields set to show on customer and contact records.
        
    -   Custom entity fields with names that match custom transaction fields that are applied to opportunities.
        
    -   Custom entity fields with names that match CRM custom fields that are applied to tasks.
        
3.  For any additional fields:
    
    1.  Select the custom field you want to map in the **Custom Lead Field** column.
        
    2.  Choose the custom fields in the columns for contacts, opportunities, and tasks that you want to map the custom lead field to.
        
    3.  If you don't want the information in the lead field to be included in one of these other records, don't select a mapped field for that record type.
        
    4.  Repeat these steps for each custom lead field you want to map.
        
4.  Click **Save**.
    

When you convert the lead record, NetSuite copies the information in the mapped custom fields to the fields on the contact, opportunity, and task.

If you delete a custom field on your lead form, you lose all of your mapping information for that field. You also lose your mapping if you change the type of custom field (from text field to a date field, for example). If you remove the custom field from a record, NetSuite keeps the mapping but the data is hidden. If you later add the field to the record again, NetSuite restores the mapping automatically.

### Related Topics

-   [Lead Conversion Using the Lead Conversion Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1086741.html)
-   [Converting a Lead on the Convert Lead Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162733129047.html)
-   [Lead Conversion Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1090008.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
