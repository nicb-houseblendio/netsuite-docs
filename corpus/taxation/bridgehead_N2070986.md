---
id: "bridgehead_N2070986"
type: "bridgehead"
title: "Setting Up Default Nature of Transaction Codes on Transaction Records"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > European Union (EU) Tax Topics > EU Intrastat Report > Intrastat Reporting Fields > Nature of Transaction Code > Setting Up Default Nature of Transaction Codes on Transaction Records"
parent: "section_N2070738"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2070986.html"
anchors: ["procedure_N2070904", "subsect_164379345533"]
sha256: "7fc2e635a2b0add97b4d1308bc3333c4dbb87526c8968f1d686ca3d2f2c397ab"
---

You can set default Nature of Transaction Codes (NoTC) for bills, cash refunds, cash sales, checks, credit memos, invoices, purchase orders, and sales orders. The system automatically selects the default NoTC in the **Nature of Transaction Code** field when you create a transaction record for the nexus. If you create a purchase or sales order and process it up to the creation of a credit memo or invoice, the NoTC value is retained.

Important:

In some countries, tax agencies don't let you to edit transaction records, so be sure to select the correct code before saving the transaction.

#### To set a default nature of transaction code for a transaction type: {#procedure_N2070904}

1.  Go to Setup > Accounting > Manage Tax Reporting.
    
2.  Click the **Intrastat Defaults** subtab.
    
3.  Select a nexus.
    
4.  Select a nature of transaction code from the **NOTC** dropdown list.
    
    Note:
    
    The dropdown list shows the codes saved on the **Intrastat Reporting** subtab.
    
5.  Select the transaction type in which this code should appear by default. You can assign multiple transaction types for one NoTC. Hold the CTRL key to select multiple transaction types.
    
6.  Click **Add**.
    

## Inactivating Default NoTC {#subsect_164379345533}

If you want to change the default NoTC for a transaction type, you need to inactivate or delete the old default NoTC first before adding a new one. If you inactivate or delete a default NoTC, the Nature of Transaction Code field on the Tax Reporting subtab will be blank for new transactions only. Changing a default NoTC doesn't affect earlier transactions.

#### To inactivate or delete a default nature of transaction code:

1.  Go to Setup > Accounting > Manage Tax Reporting.
    
2.  Click the **Intrastat Defaults** subtab.
    
3.  Check the box beside the Default Nature of Transaction Code to be deleted.
    
4.  Click **Inactivate**.
    

### Related Topics:

-   [Nature of Transaction Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2070738.html)
-   [Setting Up Nature of Transaction Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2070762.html)
-   [Creating a Nature of Transaction Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164379251413.html)
-   [Country-Specific Nature of Transaction Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1504850148.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
