---
id: "section_N2368449"
type: "section"
title: "Preferred Transaction Delivery on Vendor Records"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Records > Vendor Record Configuration > Preferred Transaction Delivery on Vendor Records"
parent: "article_161952107343"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2368449.html"
anchors: ["procedure_N2368512", "bridgehead_N2368615", "bridgehead_N2368646"]
sha256: "4093d1f23b21bba53c3a1256453e1a8c006f0e920835b1e666f70f7883817800"
---

Each vendor can have an individual preference for how to receive transactions. You can set a preferred transaction delivery method on their record as the default way to deliver transactions to them. You can choose regular mail (printing), email, fax, or a combination of the three. Then, the preferred delivery method for the vendor is marked by default in the following situations:

-   on transactions when you select that vendor
    
-   on transactions created from that vendor record
    
-   on transactions that are copied or converted from a transaction that uses these settings
    
    For example:
    
    -   You click Make Copy on a bill when this vendor is selected on the transaction. The delivery preferences default from the vendor record on the new copy of the bill.
        
    -   You click Bill on a purchase order when this vendor is selected on the purchase order. The delivery preferences default from the vendor record on the bill that is created.
        

#### To define the preferred transaction delivery method on vendor records: {#procedure_N2368512}

1.  Go to _Lists > Relationships > Vendors_.
    
2.  Click **Edit** next to the vendor whose record you want to update.
    
3.  Click the **Preferences** subtab.
    
4.  Next to **Send Transactions Via**, check the appropriate boxes:
    
    -   **Email** - Check this box to check the To Be Emailed box by default on transactions when this vendor is selected.
        
    -   **Print** - Check this box to check the To Be Printed box by default on transactions when this vendor is selected.
        
    -   **Fax** - Check this box to check the To Be Faxed box by default on transactions when this vendor is selected.
        
5.  Click **Save**.
    
    After you save these settings on the vendor record, these boxes are checked by default.
    
    Note:
    
    These settings override any customized settings on transaction forms you use.
    

## Default Methods for All Vendor Records {#bridgehead_N2368615}

You can enable preferences that set initial default transaction delivery methods for all new vendor records you create. Later, you can change the settings on individual vendor records as needed by checking or clearing the appropriate boxes. Then, the settings indicated on each vendor record will default on transactions created for that vendor.

For example, you can set a preference that when a new vendor is entered, they default to only having the To Be Emailed box checked. If a vendor also wants their transactions faxed to them, you can edit that vendor record and check the To Be Faxed box.

#### To set initial default values for print or fax:

1.  Go to _Setup > Company > Preferences > Printing & Fax_.
    
2.  On the Printing subtab or Fax subtab, check the **Vendors Default to** \[Print/Fax\] **Transactions** box
    

#### To set email as the initial default value for transactions:

1.  Go to _Setup > Company > Email > Email Preferences_.
    
2.  Check the **Vendors Default to Email Transactions** box.
    
    For more information, see [Setting Printing and Fax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N253916.html).
    

## Mass Update Vendor Records {#bridgehead_N2368646}

#### To set values using mass update:

1.  Go to Lists > Mass Updates > Mass Updates > General
    
2.  Click **Vendor**.
    

For more information, see [Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1103335211.html).

### Related Topics

-   [Vendor Record Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161951406143.html)
-   [Enabling the Vendor Access Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161952527878.html)
-   [The Vendor Center Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2369118.html)
-   [Assigning a Role to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2363606.html)
-   [Giving Vendors Access to Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2364581.html)
-   [Vendor Records for 1099 Contractors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2364122.html)
-   [Vendor Credit Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2365918.html)
-   [Associating a Vendor With an Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2367376.html)
-   [Associating a Vendor With a Payroll Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2367472.html)
-   [Importing a Vendor Price List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2368077.html)
-   [The Multiple Vendors Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2369578.html)
-   [Vendor Record Configuration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161952107343.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
