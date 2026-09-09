---
id: "section_N1747534"
type: "section"
title: "Working with Estimated Selling Prices"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > EITF 08-01 Revenue Recognition Feature > Working with Estimated Selling Prices"
parent: "chapter_N1742394"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1747534.html"
anchors: ["procedure_N1748811", "bridgehead_N1748877", "bridgehead_N1748894", "bridgehead_N1749573", "procedure_N1749590", "procedure_N1749633", "bridgehead_N1749679", "bridgehead_N1749710", "bridgehead_N1749723"]
sha256: "307fec4cfd9e1f53e0942ae6fc06e50b0e566dabdfef1a3d6bd55a8b2272b7c1"
---

Important:

EITF 08-01 Revenue Recognition is a managed SuiteApp (Bundle ID: 29321).

You add or modify the estimated selling prices for an item on the item record.

#### To add or modify estimated selling prices: {#procedure_N1748811}

1.  Go to Lists > Accounting > Items.
    
2.  Click **Edit** next to the item you want to modify.
    
3.  Click the **Custom** subtab.
    
4.  Select an **Item Category** for the item. Item categories determine how an item is sold and processed on new and renewal transactions.
    
    -   Perpetual items, such as on-premise software installations, aren't renewed and are paid in full up front. Examples of perpetual items include:
        
        -   **License - Perpetual**
            
        -   **Services**
            
        -   **Training**
            
        -   **Other**
            
        -   **Hardware**
            
    -   Term-based items have a start date and an end date. For it to be priced correctly on new and renewal transactions, term-based items must be set up with a monthly price based on the term in months of the transaction line. Examples of term-based items include:
        
        -   **License - Term**
            
        -   **Services**
            
    -   Maintenance and Support (M/S) contracts are linked to licenses. M/S pricing can be calculated as a percentage of license or can be itemized and sold based on configuration. Both must also be set up with a monthly pricing rate.
        
        -   **Maintenance - New** and **Maintenance - Renewal** - Maintenance contracts are linked to perpetual licenses and provide software updates and support for the software.
            
        -   **Support - New** and **Support - Renewal** - Support contracts are linked to term licenses and provide support for the software.
            
    
    Take note of the following:
    
    -   Items under Services or Training categories are evaluated for contingent revenue handling.
        
    -   Services, Training, Other, and Hardware item categories don't consider renewals, unless customizations have been applied.
        
5.  Select **Item Options**, if available.
    
6.  To add new estimate prices by dimension combination:
    
    1.  Click **New Multiple Allocation Price**.
        
    2.  On the New Multiple Allocation Price page, enter the ESP price and select the dimensions it applies to. Add notes or a description of the price source in the **Memo** field.
        
7.  To modify an existing estimated selling price, on the **Custom** subtab of the item, click **Edit** for the price you want to change and make changes as needed.
    
8.  To add an existing estimated selling price to the item, on the **Custom** subtab, select a price ID from the **Multiple Allocation Price** list. Click **Attach** to add the price to the item.
    
9.  Click **Save**.
    

## Using Estimated Selling Price Ranges {#bridgehead_N1748877}

With EITF 08-01 Revenue Recognition, you have the option to use a range of estimated selling prices to determine the item allocation price on a transaction. When you establish an estimated selling price range for an item, you define the limits for an allowable price variance. The sales order price on a transaction will be used for the allocation price if the sales order price falls within the specified range of the ESP price. If the sales order price isn't within the ESP price range, then the ESP price becomes the allocation price on the order. Using price ranges can help reduce the number of ESP prices maintained on the Multiple Allocation Price List.

To establish price ranges, set the upper and lower price limits for an ESP item on the item record or the Multiple Allocation Price List. You can define range limits for ESP items as needed. You don't have to define a price range for all items as the default values for both the lower and upper limits are zero percent. The price range limits determine how much the sales order price for an item can vary from the item's estimated selling price and still be used as the allocation price for calculating revenue allocation. By using percentages rather than amounts to define the price range, you don't have to update the price range limits if you change the ESP Price for an item.

## Estimated Selling Price Range Example {#bridgehead_N1748894}

ABC Software sells software and related professional services to its customers. The Multiple Allocation Price List below shows the ESP pricing details for some of their products:

| Multiple Allocation Price List |
| --- |
| ESP Item | ESP Price | ESP Price % Lower Limit | ESP Price % Upper Limit | IsVSOE | Currency |
| --- | --- | --- | --- | --- | --- |
| Hardware | 310.00 | 5.0% | 10.0% | No | USD |
| Tech Support | 200.00 | 5.0% | 10.0% | No | USD |
| Setup Services | 500.00 | 5.0% | 10.0% | No | USD |
| Software License | 1000.00 | 10.0% | 10.0% | Yes | USD |
| Software Upgrade | 990.00 | 0.0% | 0.0% | No | USD |

On one sales order, Tech Support is billed at $210.00. On another order, the sales price is $175.00. Based on the Multiple Allocation Price List, the price range for Tech Support is $190.00 to $220.00. The Allocation Amount for the Tech Support items is shown in the table below:

|  | ESP Item | Sales Order Price | ESP Price Range | Allocation Price |
| --- | --- | --- | --- | --- |
| Sales Order 1 | Tech Support | 210.00 | 190.00 to 220.00 | 210.00 |
| Sales Order 2 | Tech Support | 175.00 | 190.00 to 220.00 | 200.00 |

When the sales order price ($210.00) falls within the ESP Price Range, the Allocation Price is the sales order price, $210.00. When the sales order price ($175.00) isn't within the ESP Price Range, the Allocation Price is the ESP Price, $200.00.

## Setting Up ESP Price Ranges {#bridgehead_N1749573}

To use price ranges, enable the **Apply Price Range** preference.

When you enable this preference, EITF 08-01 determines if the item sales price is within the defined ESP price range and sets the allocation price accordingly. If this preference isn't enabled, the price ranges are ignored and the ESP price for the item is used for the allocation price. By default this preference is disabled.

#### To enable price ranges: {#procedure_N1749590}

1.  Go to _Setup > Preferences > General Preferences_.
    
2.  On the **Custom Preferences** subtab, check the **Apply Price Range** box.
    

#### To enter price ranges: {#procedure_N1749633}

1.  Go to Lists > Accounting > Items, and then select an item.
    
2.  On the **Custom** subtab, select an **ESP Price**.
    
3.  In the **ESP Price % Lower Limit** field enter a percentage of the ESP Price amount to establish the lower limit price range. If the price entered on a sales order for this item is within the range limits, the sales order item price will be used for allocation.
    
4.  In the **ESP Price % Upper Limit field**, enter a percentage.
    
5.  Click **Save**.
    

## Using IsVSOE {#bridgehead_N1749679}

When you set up the multiple allocation price list for an item, check the IsVSOE box to use the VSOE price as the estimated selling price for the item. The VSOE price is available for specific sales dimensions. When IsVSOE isn't checked, the Estimate box is checked in the VSOE Allocation field group, as shown below.

![Screenshot of VSOE Allocation field group with Estimate box checked](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/RevenueExpenseRecognition/Estimatechecked.png)

## Previewing Allocation Information {#bridgehead_N1749710}

In EITF 08-01 Revenue Recognition, you can generate allocation prices for information purposes without allocating the amounts by enabling the **Always Calculate EITF-08-01** preference. Set this preference if you want to be able to preview the allocation results generated from using the EITF 08-01 rules to recognize revenue. When you save a sales order with this preference enabled, the **Allocation Price** and **Calculated Amount** fields are populated in the **VSOE** field for transaction lines. This lets you preview the calculate amount values. The **Allocation Amount** field is blank indicating that the revenue hasn't been allocated for the transaction. By default, this preference isn't enabled. Contact Professional Services for more information if you're interested in using this preference.

## Setting Up Custom ESP {#bridgehead_N1749723}

Important:

Contact Professional Services if you want to enable the Custom ESP functionality.

You can use a custom value for an item's ESP price instead of retrieving the ESP from the Multiple Allocation Price record for the item. The Custom ESP preference is indicated in the item record by the **Custom ESP** box on the Custom subtab.

Enabling the Custom ESP functionality requires a custom function that will determine the Custom ESP value.

#### To set up Custom ESP:

1.  Add the custom function to an existing script file, or create a new script file and upload it to the file cabinet.
    
2.  If you uploaded a new script file, create a client side script record.
    
    For more information, see [Creating a Script Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489062315.html).
    
3.  Deploy the script to transaction records (Cash Sale, Invoice, Return Authorization, Sales Order).
    
    For more information, see [Methods of Deploying a Script](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4519293976.html).
    
4.  Modify Custom ESP preferences:
    
    1.  Go to Customization > Lists, Records, & Fields > Record Types.
        
    2.  On the Record Types page, click the **List** link for **EITF 08-01 Preferences**.
        
    3.  Edit and enter a preference value for the following:
        
        -   **Custom ESP File ID** - Enter the internal ID of the script you uploaded to the file cabinet.
            
        -   **Custom ESP Function Name** - Enter the name of the function that will run during server side operations, such as CSV Import, Web Service, and other non-UI contexts.
            
        -   **Custom ESP Client Function Name** - Enter the name of the function that will run during client side operations, such as UI context.
            
    4.  Click **Save**.
        

### Related Topics

-   [EITF 08-01 Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1742394.html)
-   [Understanding EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1742630.html)
-   [EITF 08-01 Allocation Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1743302.html)
-   [Contingent Revenue Handling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1743516.html)
-   [About Installing EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746114.html)
-   [Implementing EITF 08-01 Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1746357.html)
-   [Applying EITF 08-01 Scripts to Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0806035426.html)
-   [How Can I Get This Feature?](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1749904.html)
-   [Revenue and Expense Recognition Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1675871.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
