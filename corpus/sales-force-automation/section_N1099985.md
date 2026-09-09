---
id: "section_N1099985"
type: "section"
title: "Printing Mailing and Shipping Labels"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Record Management > Printing Mailing and Shipping Labels"
parent: "chapter_N1074872"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1099985.html"
anchors: ["procedure_N1100065"]
sha256: "dda80fefc10498cdac75af315c91246665adb65ec8e62771143ac607d08d0062"
---

You can print mailing or shipping labels for customers, vendors, partners, employees, or contacts without using mail merge or data export. You can use a group or saved search in the mailing label queue and generate labels for all of them at one time.

The standard mailing label layout matches Avery 5160 and 5260 labels (2 5/8' x 1', 30 labels per page). You can generate up to 500 labels at a time. You can customize these standard label sizes to suit your individual business requirements using the Template Editor in Advanced Templates. For more information, see [Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453550706.html) and [Reviewing Available Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2863143.html).

Shipping labels include a return address, but mailing labels don't.

#### To print mailing or shipping labels: {#procedure_N1100065}

1.  Go to _Transactions > Management > Print Checks and Forms_.
    
2.  Click **Mailing Labels**.
    
3.  In the **Type** field, choose the kind of entity you want to print labels for, such as **Partners**.
    
4.  The **Starting Label** field shows the position on the label page to start printing.
    
    For example, enter a 1 to begin printing on the first label or enter 4 to start printing on the fourth label.
    
5.  In the **No. of Labels** field, enter how many labels you need for each entity.
    
    For example, if you need 2 labels for each customer, enter 2.
    
    Note:
    
    You can queue and print a total of 500 labels at one time.
    
6.  In the **Label Type** field, choose the type of label you want to print: **Mailing** or **Shipping**.
    
    -   Choose **Mailing** if you want the label to include only the address of the receiving entity.
        
    -   Choose **Shipping** if you want the label to include the address of the receiving entity **and** your return address.
        
7.  In the **Address Type** field, select the address type you want to use on labels for this entity: **Billing** or **Shipping**.
    
    -   Select **Billing** to print the default billing address for the entity on these labels.
        
        Note:
        
        If you chose **Employee** as the entity type, you can't select Billing here. Employees can show only the Shipping address.
        
    -   Select **Shipping** to print the default shipping address for the entity on these labels.
        
8.  Filter the list as needed by entering text in the **Name/Number** field, or by selecting a group or saved search.
    
9.  Check the box in the **Print** column next to each one you want to print a label for.
    
    Note:
    
    Make sure that the record has shipping address, billing address, or both. Otherwise, the label will print a blank. For more information, see [Entering an Address on a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1099791.html).
    
10.  Click **Print**.
     

### Related Topics

-   [Record Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1074872.html)
-   [Contacts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1075037.html)
-   [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html)
-   [Lead Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1086131.html)
-   [Prospect Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1096136.html)
-   [Competitors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1096618.html)
-   [Other Name Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1096940.html)
-   [Records as Multiple Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1099012.html)
-   [Tracking Time on Relationship Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1099216.html)
-   [Entering an Address on a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1099791.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
