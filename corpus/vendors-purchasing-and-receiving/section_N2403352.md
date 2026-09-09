---
id: "section_N2403352"
type: "section"
title: "Ordering Items"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Purchasing > Purchase Order Management > Ordering Items"
parent: "section_N2399585"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2403352.html"
anchors: ["procedure_N2403368"]
sha256: "90dda9a30282e9d4a53e665cf429a6a867a66b553ad6ae0d63b4909e6862b362"
---

The Order Items form provides a list of items that need to be ordered from vendors. NetSuite suggests the quantity to order based on your preferred stock level and quantity of open backorders, or quantities scheduled on blanket purchase orders. You can verify or change the suggested amounts, and then create purchase orders for those items.

#### To bulk order items: {#procedure_N2403368}

1.  Go to _Transactions > Inventory > Order Items_.
    
2.  You can limit the items that show in the lists by selecting filters in the following fields:
    
    -   **Location** - Limit items based on location.
        
        -   Select a location to show only items needed in that location that are at or below their reorder point.
            
        -   Select **All** to show items from all locations that are at or below their reorder point.
            
        
        Note:
        
        If you enable the Centralize Purchasing in a Single Location preference, then items won't be filtered by location. When this preference is enabled, your selection in the **Location** field determines the location that shows on purchase orders created. Set this preference at _Setup > Accounting > Preferences > Accounting Preferences_.
        
    -   **Department** - Limit items based on department.
        
    -   **Vendor** - Limit items based on vendor.
        
        -   Select a vendor to display only items that identify this vendor as the Preferred Vendor on their item record. These items are at or below their reorder point.
            
            Important:
            
            If you use NetSuite OneWorld and vendors are shared with multiple subsidiaries, **Location** must be the one assigned to the vendor's designated subsidiary. Otherwise, you can't select the Preferred Vendor from the **Vendor** list.
            
        -   Select **All** to show only items that identify any vendor as the Preferred Vendor on their item record. These items are at or below their reorder point.
            
    -   **Include Items with No Preferred Vendor** - Check this box for the ordering list to include items that have not designated a preferred vendor. Clear this box for the ordering list below to exclude items that have not designated a preferred vendor.
        
    -   **Include Items where Vendor is Not Preferred** - Check this box for the ordering list to include items from non-preferred vendors. Clear this box for the ordering list below to exclude items from vendors that are not the preferred vendor.
        
    -   **Parent Item** - Select a parent inventory item to display only the sub-items of the parent that are at or below their reorder point.
        
    -   **Minimum Quantity** - Enter a number to display only items with a Quantity To Order equal to or larger than the number you enter.
        
        For example, you enter **10** in this field. Items with a Quantity To Order equal to or greater than 10 appear in the list.
        
3.  To send purchase orders to your vendors when you submit the form, check the appropriate box to print, email or fax the order.
    
4.  Complete steps for the **Time Phased Items** subtab, **Reorder Point Items** subtab, and **Blanket PO Items** subtab, as described in the following sub-topics.
    
5.  After all lines on all subtabs are completed as necessary, click **Submit** to place the orders.
    

After you click Submit, NetSuite generates one purchase order per vendor for the items. The orders are printed, emailed, or faxed to your vendors as indicated in the header.

For the current status, view or refresh the Status page at _Transactions > Inventory > Order Items > Status_ > Status. For more information, see [Order Items Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4714342508.html).

#### Time Phased Items Subtab

Note:

Take note of the following:

-   To use these enhancements for time-phased planned items on the Order Items page, the Demand Planning feature must be enabled.
    
-   The Time Phased Items subtab shows a list of items that need to be ordered based on time-phased replenishment. These items have a quantity available that is less than the reorder point indicated on the item record.
    

1.  **Order Start Date** - Choose to filter by the order start date.
    
2.  **Order End Date** - Choose to filter by the order end date.
    
3.  Check the box next to each item to order.
    
    Click the **Mark All** button to check all boxes or click the **Unmark All** button to clear all boxes.
    
4.  Verify or select the appropriate **Vendor**.
    
5.  Accept the suggested amount to order in the **Quantity** column or enter a new quantity.
    
    Note:
    
    For information about suggested quantities if you use the Demand Planning feature, see [Demand Planning on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2289082.html).
    
6.  If a qualified contract exists, the one with the lowest item base rate is displayed in the **Purchase Contract** field.
    
    The base rate is displayed in the **Order Rate** field.
    
7.  If you use the accounting preferences **Make Departments Mandatory** and **Allow Per-Line Departments**, verify the appropriate **Department**. The departments set on these line items are used for the corresponding line items on generated purchase orders. For more information, see [Using Per-Line Classifications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N265988.html).
    
8.  If you use the Multiple Currencies feature, each vendor's primary currency is used on this transaction. For more information, see [Vendors and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1400742.html).
    
9.  The **Total** field displays the amount calculated as Rate x Quantity.
    
    The **Total** field in the header of the Order Items page displays the sum of the **Total** column. It is updated after any change to the values in the **Total** column.
    
10.  If you use the Multiple Currencies feature, the **Total (Foreign Currency)** field displays the total calculated as Rate (Foreign Currency) x Quantity.
     

#### Reorder Point Items Subtab

1.  In the **Replenishment Method** field, filter the list of orders to show only items using a certain replenishment method. Select the Time Phased method, the Reorder Point method, or select All to show all items regardless of the replenishment method used.
    
    Note:
    
    To use these enhancements for time-phased planned items on the Order Items page, the Advanced Inventory Management feature must be enabled.
    
    The Reorder Point Items subtab shows a list of items that need to be ordered based on designated reorder point. These items have a quantity available that is less than the reorder point indicated on the item record.
    
2.  Check the box in the **Order** column next to items you want to order.
    
    Click the **Mark All** button to check all boxes or click the **Unmark All** button to clear all boxes.
    
    When NetSuite creates purchase orders from the Order Items page, it uses the Standard Purchase Order form to create the orders. When you open or edit a purchase order, NetSuite still shows your preferred form. To avoid errors, make sure your role has access to the Standard Purchase Order form
    
3.  Verify or select the appropriate **Vendor**.
    
4.  Accept the suggested amount to order in the **Quantity** column, or enter a new quantity.
    
    The quantity NetSuite suggests to order is calculated as:
    
    (preferred stock level + quantity needed) less (quantity available + quantity on order)
    
5.  If a qualified contract exists, the one with the lowest item base rate is displayed in the **Purchase Contract** field.
    
    The base rate is displayed in the **Order Rate** field.
    
6.  If you use the accounting preferences **Make Departments Mandatory** and **Allow Per-Line Departments**, verify or select the appropriate **Department**. The departments set on these line items are used for the corresponding line items on generated purchase orders. For more information, see [Using Per-Line Classifications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N265988.html).
    
7.  If you use the Multiple Currencies feature, each vendor's primary currency is used on this transaction. For more information, see [Vendors and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1400742.html).
    
8.  The **Total** field displays the amount calculated as Rate x Quantity.
    
    Note:
    
    The **Total** field in the header of the Order Items page displays the sum of the **Total** column. It is updated after any change to the values in the **Total** column.
    
9.  If you use the Multiple Currencies feature, the **Total (Foreign Currency)** field displays the total calculated as Rate (Foreign Currency) x Quantity.
    

#### Blanket PO Items Subtab

1.  **Order Start Date** - Choose to filter by the order start date.
    
    Note:
    
    Take note of the following:
    
    -   To use these enhancements for time-phased planned items on the Order Items page, the Blanket Purchase Orders feature must be enabled.
        
    -   The Blanket PO Items subtab shows blanket purchase order schedules that are within the lead time of items that need to be ordered.
        
    
2.  **Order End Date** - Choose to filter by the order end date.
    
3.  Check the box in the **Order** column next to items you want to order.
    
    Click the **Mark All** button to check all boxes or click the **Unmark All** button to clear all boxes.
    
4.  Verify or select the appropriate **Vendor**.
    
5.  Accept the suggested amount to order in the **Quantity** column, or enter a new quantity.
    
    The quantity NetSuite suggests to order is based on the blanket purchase order schedule.
    
6.  If you use the Multiple Currencies feature, each vendor's primary currency is used on this transaction. For more information, see [Vendors and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1400742.html).
    
7.  If you use the accounting preferences **Make Departments Mandatory** and **Allow Per-Line Departments**, verify or select the appropriate **Department**. The departments set on these line items are used for the corresponding line items on generated purchase orders. For more information, see [Using Per-Line Classifications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N265988.html).
    

Note:

If you have multiple locations and do not use the Centralize Purchasing in a Single Location preference, one purchase order is created per location. Set this preference at _Setup > Accounting > Preferences > Accounting Preferences_.

If you use the Centralize Purchasing in a Single Location preference, you can distribute items you receive to your locations. Go to one of the following:

-   _Transactions > Inventory > Transfer Inventory_.
    
-   _Transactions > Inventory > Replenish Location_.
    

### Related Topics

-   [Setting Purchasing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2400174.html)
-   [Entering a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2400504.html)
-   [Bulk Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2402825.html)
-   [Billing a Purchase Order With Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2403862.html)
-   [Editing a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2404305.html)
-   [Viewing the Status of a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2408514.html)
-   [Printing a Tax ID or Resale Number on Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4746558953.html)
-   [Purchase Order Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2407704.html)
-   [Purchase Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2399585.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
