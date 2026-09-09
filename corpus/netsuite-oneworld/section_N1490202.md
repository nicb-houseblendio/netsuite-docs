---
id: "section_N1490202"
type: "section"
title: "Creating Intercompany Customers and Vendors"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Setting Up Automated Intercompany Management > Creating Intercompany Customers and Vendors"
parent: "section_N1486610"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1490202.html"
anchors: ["procedure_N1490396", "procedure_N1490486"]
sha256: "d4aa2d1b145f6d21d38fa9fa5d627d0f51449e84c8a2aca9b0d3cd1b8d99a702"
---

Intercompany customers and vendors are entity records with one or more assigned subsidiaries that NetSuite uses for intercompany transactions. They represent the buyer and seller in transactions between subsidiaries. The default receivable account for an intercompany customer must be an intercompany receivable account. For intercompany vendors, the default payable account must be an intercompany payable account.

Important:

Prior to NetSuite 2020.2, the Automated Intercompany Management feature required users to customize the vendor and customer records to include the **Represents Subsidiary** field. This field indicates that the entity acts as an agent for a selected subsidiary. After you customized the entity forms, you then manually created intercompany vendors and intercompany customers to represent your non-elimination subsidiaries. When you changed a subsidiary record, you were required to manually update the representing entity records.

In 2020.2, NetSuite provides functionality that creates and maintains system-generated representing entities. However, there are prerequisites to take advantage of this functionality. You must enable the Multi Subsidiary Customer feature. In addition, if you use the Multiple Currencies feature, you must also enable the Multi-Currency Vendor and Multi-Currency Customer features. If you meet these prerequisites, NetSuite can generate and maintain representing entities for all of your non-elimination subsidiaries. For more information, see [Intercompany Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1549982657.html) and [Representing Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159067444188.html).

You enter intercompany entities on sales orders and purchases orders to create intercompany transactions. You can also identify an intercompany customer or vendor on journal lines when you create an advanced intercompany journal entry. You must enter an intercompany entity for lines that include an intercompany receivable or intercompany payable account. For information about setting up intercompany accounts, see [Intercompany Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486928.html).

## Intercompany Customer and Corresponding Intercompany Vendor Example

You can manually create an intercompany customer and corresponding intercompany vendor for each subsidiary-to-subsidiary relationship that has intercompany transactions. For example, if Subsidiary U.K. purchases a product from Subsidiary U.S., create the following entities to represent the subsidiaries:

-   Create a customer record in Subsidiary U.S. to represent Subsidiary U.K. (the buyer).
    
    -   Subsidiary = U.S. Subsidiary
        
    -   Represents Subsidiary = Subsidiary U.K.
        
-   Create a vendor record in Subsidiary U.K. to represent Subsidiary U.S. (the seller).
    
    -   Subsidiary = Subsidiary U.K.
        
    -   Represents Subsidiary = Subsidiary U.S.
        

An entity record can act as an agent for only one subsidiary. If Subsidiary U.K. also purchases from Subsidiary EU, you must:

-   Create a customer record in Subsidiary EU to represent Subsidiary U.K. (the buyer).
    
    -   Subsidiary = EU Subsidiary
        
    -   Represents Subsidiary = Subsidiary U.K.
        
-   Create a vendor record in Subsidiary U.K. to represent Subsidiary EU (the seller).
    
    -   Subsidiary = Subsidiary U.K.
        
    -   Represents Subsidiary = Subsidiary EU
        

Before you can manually create intercompany customers and vendors, you must customize the customer and vendor forms to include the **Represents Subsidiary** field. To customize forms, go to _Customization > Forms > Entry Forms ( Administrator )_. Add the **Represents Subsidiary** field to the standard customer and standard vendor forms. For information about customizing forms, see [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html) and [Configuring Fields or Screens](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856992.html).

#### To manually create intercompany customers: {#procedure_N1490396}

1.  Go to _Lists > Relationships > Customers > New_.
    
2.  In **Custom Form**, select your custom intercompany customer form.
    
3.  Enter the information for the intercompany customer including:
    
    -   **Company Name:** Use a naming convention to identify this as an intercompany entity such as U.S. Customer in Canada Sub.
        
    -   **Subsidiary:** Select the subsidiary to which this entity belongs.
        
    -   **Represents Subsidiary:** Select the subsidiary that the entity represents.
        
4.  On the **Financial** subtab, for **Default Receivables Account**, select an intercompany receivable account from the list.
    
    This is the default intercompany receivables account for the customer.
    
5.  Complete other information as needed for the customer.
    
6.  Click **Save**.
    

For information about multiple subsidiaries assigned to a customer record, see [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).

#### To manually create intercompany vendors: {#procedure_N1490486}

1.  Go to _Lists > Relationships > Vendors > New_.
    
2.  In **Custom Form**, select your custom intercompany vendor form.
    
3.  Enter the information for the intercompany vendor including:
    
    -   **Company Name:** Use a naming convention to identify this as an intercompany entity such as U.S. Vendor in Canada Sub.
        
    -   **Subsidiary:** Select the subsidiary to which this entity belongs.
        
    -   **Represents Subsidiary:** Select the subsidiary that the entity is representing.
        
4.  On the **Financials** subtab, or **Default Payables Account**, select an intercompany payable account from the list.
    
    This is the default intercompany payable account for the vendor.
    
5.  Complete other information as needed for the vendor.
    
6.  Click **Save**.
    

For information about multiple subsidiaries assigned to a vendor record, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).

### Related Topics:

-   [Account Types and Intercompany Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1487157.html)
-   [Creating Intercompany Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1489768.html)
-   [Intercompany Inventory Items Guidelines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1490669.html)
-   [Customizing Standard Journal Entries for Intercompany Elimination](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492223.html)
-   [Setting Up Automated Intercompany Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486610.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
