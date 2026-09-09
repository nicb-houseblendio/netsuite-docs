---
id: "section_N1226924"
type: "section"
title: "Bulk Fulfilling Orders Using a CSV Import"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Order Fulfillment > Fulfilling Orders > Bulk Fulfilling Orders Using a CSV Import"
parent: "section_N1223349"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1226924.html"
anchors: ["procedure_N1226947"]
sha256: "7f67a0b22a404afef9cabb7929626e09d52d14d4b38805698269713aa5b69f00"
---

Bulk fulfill orders by importing a CSV file with fulfilled order numbers. Like bulk fulfilling on the Fulfill Orders page, you choose the accounting posting period for the orders, the transaction date, and a shipment status (if the Pick, Pack, and Ship feature is enabled). You can also select the bulk fulfill location if the Multi-Location Inventory feature is enabled.

The required CSV fields depend on your NetSuite account's preferences and features.

-   The Charge for Shipping preference.
    
-   The Advanced Shipping feature.
    
-   The Multi-Location Inventory feature.
    
-   Shipping integration with FedEx, UPS, or USPS.
    

Download a sample CSV file to see the required fields. If a field is in the sample file for your company, you must include it in the CSV file to be imported. For example, if you charge for shipping, but don't use the Advanced Shipping feature nor shipping integration, the CSV file has two fields only: Order Number and Tracking Number.

To download a sample CSV, go to _Transactions > Order Management > Fulfill Orders_ and click the Import-CSV button. Click the link next to the File field to download a sample file.

Here are the possible CSV fields:

| Field | Description |
| --- | --- |
| Order Number | The order number as it appears in NetSuite. If order numbers have prefixes, you must include the prefix, for example, 'SO160089' instead of '160089'. |
| Transaction Type | This field must be one of the following transaction types:
-   Sales Order
-   Transfer Order

 |
| Weight | The total weight of the order. |
| Tracking Number | The tracking number of the package. 64 digits maximum. |
| Label Integration | A boolean value indicating the sales order uses label integration. This field must be one of the following values:

-   T
-   F

T (True) indicates the sales order uses label integration. F (False) indicates the sales order does not use label integration. |

The first line in the CSV file must be a header line with the exact field names from the sample file. You can't upload the CSV file without the header line or with incorrect field names. For information about naming and formatting CSV files, see [General CSV File Conventions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453326.html).

Note:

Columns and custom fields cannot be added to this type of import.

#### To bulk fulfill orders using a CSV Import: {#procedure_N1226947}

1.  Go to _Transactions > Order Management > Fulfill Orders_.
    
2.  On the **Fulfill Orders** page, click the **Import-CSV** button to open the Import CSV page.
    
3.  If you need to prepare a CSV file, click the link next to the File field to download a sample file. You can enter information in this file or create a file like it.
    
    Note:
    
    The first line (header) in the sample file lists the required fields. A brief explanation of the fields is shown below the first line. To use the file, delete all lines in the sample file except the first line and then enter the fulfillment information in the file.
    
4.  In the **File** field, select the CSV file containing the list of fulfilled orders you want to import.
    
5.  Enter a posting period and a date.
    
6.  If the Pick, Pack, and Ship feature is enabled, select a value for **Set Shipment Status To**. If the CSV import process is completed successfully, the status of the item fulfillment is set to the value you selected in the Set Shipment Status To field.
    
7.  If Multi-Location Inventory is enabled, select a location in the **Bulk Fulfill from Location** dropdown.
    
8.  If the Advanced Shipping feature is enabled, select a value for **Ship Via**.
    
9.  To specify the values for other fields in the orders, select a field in the Field column and enter the value in the Selection, Checked, Text, or Date columns. The value you specify will be used for all orders in the CSV file.
    
10.  Click **Submit**.
     
     When you click Submit, the Process Status page shows the submission status of the CSV import process. Click the **Refresh** button to update the status. When the status is Complete, you can view the results of the import. See [Checking the Processing Status of Bulk Fulfilled Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231493.html) for more information about the Process Status page.
     

When working with a third-party logistics service, you typically need to send a list of orders to the third-party before the orders can be processed and fulfilled in bulk. You can export a list of orders from NetSuite to a CSV file. To export a list of sales orders, go to _Transactions > Sales > Enter Sales Orders > List_. Filter the list of orders as required and then click the Export - CSV icon. For more information about exporting to CSV, see [Exporting Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495079.html).

### Related Topics:

-   [Checking the Processing Status of Bulk Fulfilled Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1231493.html)
-   [Order Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1222915.html)
-   [Fulfilling Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1223349.html)
-   [CSV Imports Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N342646.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
