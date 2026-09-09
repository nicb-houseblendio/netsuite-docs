---
id: "section_N1267302"
type: "section"
title: "FedEx"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > FedEx"
parent: "chapter_N1257369"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1267302.html"
anchors: ["bridgehead_N1267326", "procedure_N1268110"]
sha256: "65885daac8e340e98c8bbcb3b3d9715f4fbfd224df7c4fecd2c63cf725a9dd4a"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

## Registering a FedEx Account {#bridgehead_N1267326}

Adding a FedEx account to NetSuite enables you to offer FedEx real-time rates. You must have an active FedEx account to use FedEx real-time rates and integration.

If you have enabled Shipping Label Integration, you can print barcode shipping labels and receive tracking numbers.

If you charge for shipping, you can create shipping items with FedEx real-time rates. When a customer ships a purchase using FedEx, the current rate for the customer's location fills in the Amount field in your website and on transaction pages. The rate is an estimate of the final shipping cost and may vary slightly depending on the package size.

FedEx requires multi-factor authentication (MFA) to register and use your FedEx account in NetSuite. Until you complete your initial MFA registration, even for existing FedEx accounts in NetSuite, FedEx shipping label creation may fail. To authorize your account, choose one of the available methods (SMS, phone call, email, or invoice details) to receive a PIN. Then enter that PIN on the FedEx Registration page. If you can't complete PIN-based authorization, contact FedEx Customer Support to complete the process.

Note:

You must charge for shipping to use FedEx real-time rates or integration.

#### To add your FedEx account: {#procedure_N1268110}

1.  Go to _Setup > Accounting > Shipping_.
    
2.  Check the **Charge for Shipping** box.
    
3.  On the **Carrier Registration** subtab, click **Add FedEx Account**.
    
4.  Read the terms of agreement, and then select **I Accept**.
    
5.  If you use the Multiple Location Inventory feature, select the **Location** to associate this FedEx account with.
    
    You can add a separate FedEx account for each location you operate.
    
6.  Enter the **First Name** and **Last Name** of the person responsible for this FedEx account.
    
7.  Your **Company** name is displayed.
    
8.  Enter the **Department** the FedEx account contact person works in.
    
9.  Enter this location's FedEx account's address information:
    
    -   **Address**
        
    -   **City**
        
    -   **State**
        
    -   **Zip** code
        
    
    Important:
    
    Use the address exactly as it appears on the FedEx account you're registering.
    
10.  Enter the FedEx account person's contact information:
     
     -   **Phone** number
         
     -   **Fax** number
         
     -   **Pager** number
         
     -   **Email** address
         
11.  Select how you want to pass packages to FedEx in the **FedEx Dropoff Type** field.
     
12.  Select your shipping label print format in the **FedEx Label Type**.
     
13.  If your label stock is perforated select **Doctab Location**
     
     -   **None** - if there is no physical doctab
         
     -   **Top** - if the doctab is at the top of the label
         
     -   **Bottom** - if the doctab is at the bottom of the label
         
     
     Doctab Location is available for PDF (8-1/2 x 11) label types.
     
14.  Select how customers pay for receiving deliveries in the **FedEx Collect on Delivery (C.O.D.) Type** field.
     
15.  Enter your **FedEx Account Number.**
     
     Only nine-digit account numbers can be entered.
     
16.  If you have a **FedEx Ground Economy** account, check the box and then select the default hub number provided by FedEx for the location.
     
     Alternatively, to register an account that supports FedEx Ground Economy customer returns by USPS, check **FedEx Ground Economy Returns**.
     
17.  In the **Authorize your FedEx Account** section at the bottom of the page, choose one of the available authorization methods (SMS, phone call, email, or invoice details).
     
     If you choose invoice details, enter the invoice number in numerals only, as shown on the FedEx website. Do not enter letters or punctuation from formatted invoice references. For example, if your invoice shows A1-234-56, enter 123456.
     
     Note:
     
     If you choose the Contact Support method, you can bypass the PIN code requirement.
     
18.  Enter the PIN code provided by FedEx to complete authorization.
     
19.  If you enabled Hazmat/Dangerous Goods Shipping, add the contact person's information.
     
     To learn more, see [Shipping Dangerous Goods and Hazardous Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1269990.html).
     
20.  Click **Save**.
     

### Related Topics

-   [Shipping Integration with FedEx, UPS, and USPS/Endicia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263996.html)
-   [FedEx Real-Time Rates (U.S. and Canada)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268998.html)
-   [Getting Started with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268430.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
