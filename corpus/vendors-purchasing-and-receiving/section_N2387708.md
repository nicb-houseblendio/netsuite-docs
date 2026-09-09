---
id: "section_N2387708"
type: "section"
title: "Viewing the Status of a Vendor Return Authorization"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Returns > Viewing the Status of a Vendor Return Authorization"
parent: "chapter_N2386193"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2387708.html"
anchors: ["procedure_N2387727"]
sha256: "6f4dc1248eb087bf4cb312b1d1c2a638632ea4d380d1b7e5e593aaf2cd432d34"
---

Each vendor return authorization has a status that reflects where the return is in the shipping and crediting process.

Note:

Vendor Return Authorization transactions now support the Advanced PDF/HTML Templates feature.

#### To view the status of a return authorization: {#procedure_N2387727}

1.  Go to _Transactions > Purchases > Enter Vendor Return Authorizations_.
    
2.  The list shows the status of each return authorization in the Status column.
    
    Depending on whether the Advanced Shipping feature is enabled, the status of a return could be as follows:
    
    -   With **Advanced Shipping on**:
        
        -   **Pending Approval** - The return is not yet approved.
            
        -   **Pending Return** - The return is approved and pending the shipment of items to the vendor.
            
        -   **Partially Returned** - Not all items have been shipped to the vendor.
            
        -   **Pending Credit** - All items on the return are shipped to the vendor and it is pending the creation of a vendor credit. This can include partially credited returns.
            
        -   **Pending Credit/Partially Returned** - Some items on the return are shipped to the vendor. It is pending the creation of a vendor credit for shipped items.
            
        -   **Credited** - The return is completely shipped and credited.
            
        -   **Canceled** - The return has been canceled.
            
        -   **Closed** - The return is closed.
            
    -   With **Advanced Shipping off**:
        
        -   **Pending Approval** - The return is not yet approved.
            
        -   **Pending Refund** - The return is approved and is pending receipt and refund of the item.
            
        -   **Partially Credit** - The return is partially shipped and credited.
            
        -   **Credited** - The return is completely shipped and credited.
            
        -   **Canceled** - The return has been canceled.
            
        -   **Closed** - The return is closed.
            

The default status for vendor returns is set by an administrator in the Returns section on the Order Management subtab. Go to _Setup > Accounting > Preferences > Accounting Preferences_.

-   If you use the approval process for vendor return authorizations, **Pending Approval** is your default status.
    
-   If you do not use the approval process, **Pending Receipt** is your default status.
    

You can change the status for each vendor return authorization in the Status field, if needed.

You can click Show Activity on a vendor return authorization record to see what has already been shipped and credited for a return.

### Related Topics

-   [Vendor Return Authorization Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2386202.html)
-   [Creating a Vendor Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2386460.html)
-   [Creating a Vendor Return Authorization From an Existing Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162003965369.html)
-   [Approving a Vendor Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2387067.html)
-   [Canceling a Vendor Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162004032986.html)
-   [Shipping Authorized Vendor Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2387332.html)
-   [Crediting an Authorized Vendor Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2388089.html)
-   [Vendor Returns for Drop-Ship Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2391620.html)
-   [Closing a Line Item on a Vendor Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2391809.html)
-   [Vendor Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2386193.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
