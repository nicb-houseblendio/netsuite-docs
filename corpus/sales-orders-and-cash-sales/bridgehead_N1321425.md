---
id: "bridgehead_N1321425"
type: "bridgehead"
title: "Setting the Order of Contract Renewal Scripts on Transaction Records"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Software Vertical Contract Renewals > Setting Up Contract Renewals > Initial Setup Tasks for Contract Renewals > Setting the Order of Contract Renewal Scripts on Transaction Records"
parent: "section_N1321054"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1321425.html"
anchors: ["procedure_N1321439"]
sha256: "9cd731c235b17f1a9522ee8d761f8d493171fa245301d2757d78d9b261146243"
---

You can set the order of Contract Renewal scripts on transaction records by following these steps.

#### To set the order of Contract Renewal scripts on transaction records: {#procedure_N1321439}

1.  Go to _Customization > Scripting > Scripted Records (Administrator)_.
    
2.  Click the **Record** column heading to sort the list by record.
    
3.  Click **Edit** next to a record, and then do these steps:
    
    -   On the **User Event Scripts** subtab, ensure the scripts are listed in the following order:
        
        -   R02A-UES-1: Check Tran Into Log
            
        -   R02A-UES-2: Calculate Tran Lines
            
        -   R02A-UES-3: Calc In-Line Discounts
            
        
        Note:
        
        By default, these user event scripts are deployed only on the sales order transaction form. If you want to use CSV import and SOAP web services on the estimate record, you must deploy these scripts on the estimate transaction form.
        
        Note:
        
        The old scripts R01C-SS: Calculate Tran Lines and R01D-SS: Calc In-Line Discounts are no longer supported by the Contract Renewals SuiteApp, so they are disabled by default (Status = Testing, Deployed = Not Checked). These scripts are replaced by R02A-UES-2: Calculate Tran Lines and R02A-UES-3: Calc In-Line Discounts. Ensure you're using the new user event scripts on your transaction forms.
        
    -   On the **Client Scripts** subtab, make sure the scripts are listed in the following order:
        
        -   R01A-CS: HeaderAutomate&Validate
            
        -   R01B-CS: TranLinesAutomate&Validate
            
        
        Note:
        
        Make sure the client scripts are also deployed in these transaction forms: credit memo, invoice, opportunity, quote, return authorization, sales order, and estimates.
        
4.  Click **Save**.
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
