---
id: "bridgehead_N376031"
type: "bridgehead"
title: "Setting Up Custom Lists and Item Fields for Matrix Options"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Items Import > Importing Matrix Options for Items > Setting Up Custom Lists and Item Fields for Matrix Options"
parent: "section_N375701"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N376031.html"
anchors: ["procedure_N376046", "procedure_N376122"]
sha256: "7d0c3c6698307f1abae753be49902f0c0a682e04a34798acf7a3b96057bc6e26"
---

Before you import matrix items, set up a custom list and a custom item field for each matrix option. Each custom list represents a matrix option such as size or color, and includes the set of possible values for that option. Each custom item field provides an interface for display and selection of that matrix option on item forms. The matrix options that you have set up in this manner are displayed on the Import Assistant's Field Mapping page as fields to be mapped.

#### To set up a custom list for a matrix option: {#procedure_N376046}

1.  Go to _Setup > Customization > Lists > New_.
    
2.  Enter a name for the option, choose the display order for option values, check the **Matrix Option List** box, add the values that you want to be available for that option, and click **Save**.
    
    ![Matrix Option List box checked on the Custom List Edit page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/CustList_2014_2.png)
    
    For more information, see [Setting up Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2228669.html#bridgehead_N2228735).
    

#### To set up a custom item field for a matrix option: {#procedure_N376122}

1.  Go to _Setup > Customization > Item Fields > New_.
    
2.  On this page, do the following:
    
    1.  Enter the name of a custom list in the **Label** field.
        
    2.  Check the **Matrix Option** box.
        
    3.  Select the custom list from the **List/Record** list.
        
    4.  On the **Applies To** subtab check the boxes for the types of items that can have this matrix option.
        
    5.  Click **Save**.
        
        ![Custom Item Field Edit page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/CustItem_2014_2.png)
    
    For more information, see [Setting up Custom Item Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2228669.html#bridgehead_N2228884).
    

### Related Topics

-   [Importing Matrix Options for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375701.html)
-   [Item Types that Support Matrix Options Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N375858.html)
-   [Prerequisites for Importing Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N375963.html)
-   [Setting Up Your CSV File for Matrix Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N376239.html)
-   [Mapping Fields for Matrix Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N376956.html)
-   [Tips for Matrix Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N377033.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
