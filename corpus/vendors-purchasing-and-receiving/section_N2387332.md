---
id: "section_N2387332"
type: "section"
title: "Shipping Authorized Vendor Returns"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Returns > Shipping Authorized Vendor Returns"
parent: "chapter_N2386193"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2387332.html"
anchors: ["procedure_N2387356"]
sha256: "3eff5dc4f2581b9acc11d89f526e9bb8b3ac11326a6497f416fcc783661e78dc"
---

When you ship items to a vendor for an authorized return, mark the item as shipped. This status lets you track the progress of the order through the return process.

#### To mark an authorized return item as shipped: {#procedure_N2387356}

1.  Go to _Transactions > Purchases > Enter Vendor Return Authorizations_.
    
2.  Select the vendor whose authorized return you want to ship. Authorized returns for the vendor show in the list. If the authorized return you want to ship is not showing in the list, the return may need to be approved.
    
    Select **All** to show approved returns for all vendors.
    
3.  In the **Return** column, check the box next to the authorized return you are shipping to the vendor.
    
4.  Click **Submit**.
    
5.  On the Item Fulfillment page:
    
    -   verify information in the following fields:
        
        -   **Vendor** - the vendor you are sending the item to.
            
        -   **Date** - the date the return is shipped
            
        -   **Ref. No.** - the reference number of the return you are shipping
            
6.  On the **Items** subtab, in the **Quantity** column, verify or enter the number of units of each item you are shipping.
    
7.  Check the box in the **Fulfill** column next to items you are shipping.
    
8.  When you have finished, choose one of the following:
    
    -   Click **Save** to save the information.
        
    -   Click **Save and Credit** to save the information and enter a bill credit for this return. Only the amount for items you shipped will show on the bill credit.
        
    -   Click **Save and New** to save the information and enter a new authorization.
        
    -   Click **Save and Print** to save the information and print a packing slip for the return.
        
        Note:
        
        You can also print a packing slip for a vendor return by going to _Transactions > Management > Print Checks & Forms_. Click **Packing Slips and Return Forms**. Be sure to check the **Allow Reprinting** box.
        
        You can also create a custom packing slip form at _Setup > Customization > Forms > Transaction Forms_. Click **Customize** next to Standard Packing Slip. Optionally set it as the preferred packing slip by doing one of the following:
        
        -   Check the **Form is Preferred** box to use the custom form for all packing slips.
            
        -   Click **Edit** next to a custom Vendor Return Authorization in the list and click the **Linked Forms** subtab. In the **Packing Slip** field, select the custom packing slip you created.
            
    -   Click **Save and Print Label** to save the information and print a shipping label.
        
        Note:
        
        When printing a shipping label for a Vendor Return Authorization, the label Reference Number value (`label.refnumber`) is sourced from the **Ref. No.** field. All other shipping labels source the label Reference Number value from the **PO#** field.
        

Now, the items on the vendor return authorization are marked returned and your inventory is automatically updated with the items that have been shipped.

To see what has already been received and billed for a return authorization, view the return authorization record and click the Related Records subtab.

### Related Topics

-   [Vendor Return Authorization Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2386202.html)
-   [Creating a Vendor Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2386460.html)
-   [Creating a Vendor Return Authorization From an Existing Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162003965369.html)
-   [Approving a Vendor Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2387067.html)
-   [Canceling a Vendor Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162004032986.html)
-   [Viewing the Status of a Vendor Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2387708.html)
-   [Crediting an Authorized Vendor Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2388089.html)
-   [Vendor Returns for Drop-Ship Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2391620.html)
-   [Closing a Line Item on a Vendor Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2391809.html)
-   [Vendor Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2386193.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
