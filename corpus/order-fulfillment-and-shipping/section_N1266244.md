---
id: "section_N1266244"
type: "section"
title: "Printing Integrated Shipping Labels With a Thermal Printer"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > Shipping Integration with FedEx, UPS, and USPS/Endicia > Printing Integrated Shipping Labels With a Thermal Printer"
parent: "section_N1263996"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1266244.html"
anchors: ["procedure_N1266270", "procedure_N1266723", "procedure_N1267029", "procedure_N1267105"]
sha256: "29203c9a6c8ec8cec86e6c6515e89992d4db4b3e1e267f6b3608d6dee47abcee"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

The Shipping Label Integration feature enables you to print a barcode shipping label for a sales order, vendor return, or transfer order.

#### To print a label:

1.  Create a shipping item.
    
    To learn more, see [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html).
    
2.  Create a sales order with the shipping item.
    
    To learn more, see [Creating Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1216500.html)
    
3.  Fulfill the sales order.
    
    To learn more, see [Fulfilling Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1223349.html)
    
4.  To generate a shipping label, check the **Label Integration** box.
    
5.  Click **Submit**.
    

For a list of compatible thermal printers, visit [UPS.com](http://www.ups.com/content/us/en/resources/sri/pri.html) and [Fedex.com](http://www.fedex.com/us/ship-manager/software/resources/support/printer-drivers.html).

## To print labels in EPL or ZPL format using a thermal printer: {#procedure_N1266270}

ZPL format is currently supported by USPS and UPS services.

-   [To install a thermal printer driver on a Windows PC:](#procedure_N1266723).
    
-   [To set up your NetSuite account to print shipping labels in EPL or ZPL format:](#procedure_N1267029)
    
-   [To print a shipping label in EPL or ZPL format:](#procedure_N1267105)
    

#### To install a thermal printer driver on a Windows PC: {#procedure_N1266723}

1.  Install the driver according to the printer manufacturer's instructions.
    
2.  **Share the printer** on a network:
    
    1.  Go to Control Panel > Devices and Printers.
        
    2.  Open printer.
        
    3.  In **Printer Properties** select the **Sharing** tab.
        
    4.  Check the **Share This Printer** box.
        
    5.  In the **Share Name** field, enter the name of the printer.
        
        The printer name cannot contain spaces.
        
    6.  Click **OK**.
        
3.  To send the label files to the printer, **Create a batch file**:
    
    1.  Open a text editor, such as Notepad.
        
    2.  If you are printing to a local printer using a USB port, replace 'PrinterName' with the name of your printer. Do not replace 'ComputerName' with the name of your computer. It will change dynamically when the batch file runs.
        
        **Net use LPT2: \\\\%ComputerName%\\PrinterName**
        
        **Copy %1 LPT2**
        
        **Net use LPT2: /Delete**
        
    3.  If you are using a network thermal printer, replace 'Server' with the print server name. Replace 'PrinterName' with the name of your printer:
        
        **print /d:\\\\Server\\PrinterName %1**
        
    4.  Click **Save**.
        
    5.  In **Filename**, enter **label.bat**. Replace the .txt suffix with .bat.
        
    6.  In the **Save as Type** field, select **All Files**.
        
    7.  Select a **Location** to save the file to.
        
    8.  Click **Save**.
        
4.  **Add the file extension** and assign default program associations:
    
    1.  From the **Start** menu, enter **Indexing**.
        
    2.  Click **Enter**.
        
    3.  In the **Indexing Options** window, click **Advanced**.
        
    4.  Click the **File Types** tab.
        
    5.  In the **Add new extension to list** field, add **epl2** and then click **Add.**.
        
        Repeat this step for **zpl**.
        
        Completing these steps ensures that you can search for your EPL2 and .ZPL files using Windows search.
        
    
    **Setting a default program to open the batch file**
    
    Select one of the following methods to open EPL2 or ZPL files from your desktop.
    
    **Method 1**
    
    1.  Save the EPL2 or ZPL file to your desktop.
        
    2.  Right-click the saved file.
        
    3.  Click **Open With** and then **Choose default program**.
        
    4.  Click **Browse** and then locate the **label.bat** file.
        
    5.  Click **Open**.
        
    6.  Check the **Always use the selected to open this kind of file** box.
        
    7.  Click **OK**.
        
    
    **Method 2**
    
    1.  Right-click the saved **EPL2** or **ZPL** file.
        
    2.  Select **Properties**
        
    3.  In the **General** tab, click **Change**.
        
    4.  Select a program from the list or click **Browse** to select the label.bat file you saved earlier.
        

#### To set up your NetSuite account to print shipping labels in EPL or ZPL format: {#procedure_N1267029}

1.  Before fulfilling the order, go to _Setup > Accounting > Setup Tasks > Shipping_.
    
2.  Click the shipping account you want to use to print the label.
    
3.  In the **Label Type** field, select one of the following options:
    
    | **Format** | **Available Shipping Accounts** |
    | --- | --- |
    | EPL (4 x 6) | UPS, USPS |
    | EPL (4 x 8) | UPS |
    | ZPL (4 x 6) | FedEx, UPS |
    | ZPL (4 x 8) | UPS |
    | ZPLII (4 x 6) | FedEx, USPS |
    | ZPLII (4 x 8-1/2) | FedEx |
    | ZPLII (4 x 10-1/2) | FedEx |
    
4.  Click **Submit**.
    

#### To print a shipping label in EPL or ZPL format: {#procedure_N1267105}

1.  After fulfilling an order, go to _Transactions > Management > Print Checks and Forms_.
    
2.  Click **Integrated Shipping Labels**.
    
3.  To begin printing on the first label of the first sheet of labels, in the **Starting Label** field, enter **1**.
    
    Enter **2** to begin printing on the second column, or second label, on the sheet.
    
4.  Select a carrier to the print labels for.
    
    Alternatively, select **All**.
    
5.  Leave the **Single Label Per Page** box clear. This preference is for printing in PDF format.
    
6.  Optionally, select a **Location**.
    
7.  In the **Print** column, check the box next to each order you want to print a label for.
    
    -   To check the boxes for all items, click **Mark All**.
        
    -   To view the sales order, click the **Order Date**.
        
    -   To view the Item order Fulfillment, click the **Ship Date**.
        
8.  Click **Print**.
    
    A window opens with instructions on how to download your label.
    

Attach the label to the package for the order, and it is ready for drop-off or pick-up.

### Related Topics

-   [Printing Shipping Labels for Multiple Carriers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265937.html#bridgehead_N1265983)
-   [Printing FedEx Shipping Labels and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1272548.html)
-   [Printing UPS Shipping Labels and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1282339.html)
-   [Printing USPS Shipping Labels and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1285080.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
