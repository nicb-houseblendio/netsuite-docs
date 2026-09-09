---
id: "section_N1271195"
type: "section"
title: "Fulfilling Orders with FedEx Integration"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > FedEx > Fulfilling Orders with FedEx Integration"
parent: "section_N1267302"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1271195.html"
anchors: []
sha256: "43ec605d16d1205b9e4f258db335f6a6eae1aa33415698d3defc57bd32a37dc1"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

When you fulfill orders using FedEx integration, on the Item Fulfillment page, FedEx offers additional options that they may charge for.

To learn more, see [www.fedex.com](http://www.fedex.com).

#### To fulfill an order using FedEx integration:

1.  Enable the Shipping Label Integration feature:
    
    1.  Go to _Setup > Company > Enable Features_.
        
    2.  Click the **Transactions** subtab.
        
    3.  In the **Shipping & Receiving** section, check the **Shipping Label Integration** box.
        
    4.  Click **Save**.
        
2.  Ship the order with a FedEx-integrated shipping item.
    
3.  Fulfill orders with FedEx integration at _Transactions > Sales > Fulfill Orders_.
    
4.  Click the **Shipping** subtab to verify the following:
    
    -   Shipping and address information is correct
        
    -   The **Integrated Shipping Label** box is checked
        
5.  Click the **Carrier** subtab, and then select the following options:
    
    -   If you need FedEx to deliver this shipment on a Saturday, check the **Saturday Service** box. Extra charges may apply.
        
        Saturday delivery is available in the majority of U.S. cities with FedEx Priority Overnight, FedEx 2Day and FedEx SameDay services. Call 1.800.GoFedEx (1.800.463.3339) for specific enquiries.
        
        If you need FedEx to collect this shipment on a Saturday, check the **Saturday Pickup** box . Extra charges may apply.
        
    -   To alert the recipient of the expected delivery date, check the **FedEx ShipAlert** box and then enter a contact email address.
        
    -   To process the shipment today but schedule a future shipment date, enter the **Future Ship Date**.
        
        Future ship dates cannot extend beyond 10 days from the current date for FedEx Express shipments, and 90 days for FedEx Ground shipments.
        
    -   If this order should be shipped using FedEx's Signature Home Delivery service for residential addresses, check the **FedEx Home Delivery** box. The recipient must sign for the package when using this service.
        
    -   When using FedEx's Signature Home Delivery, select a **FedEx Home Delivery Type** from the following options :
        
        -   To deliver this shipment on a specified date, Tuesday through Saturday, excluding holidays, select **Date Certain**
            
        -   To deliver this shipment delivered between the hours of 5:00 pm and 8:00 pm on the scheduled delivery date, select **Evening**
            
        -   To allow the recipient to arrange a specific date and time for delivery, select **Appointment**. FedEx will contact the recipient by phone to schedule delivery
            
    -   When using FedEx Signature Home Delivery, enter the **FedEx Home Delivery Date** you want this shipment delivered.
        
    -   If Date Certain or Appointment is selected as the FedEx Home Delivery Type, enter **Delivery Instructions** for the driver. These instructions are encoded into the delivery barcode. A maximum of 64 characters is allowed.
        
    -   If this is an international freight shipment, enter a **Booking Confirmation Number**. To receive this number, contact FedEx to schedule the time and place for pick-up.
        
    -   For international shipments when a Shipper Export Declaration (SED) is required, enter a **AES/FTSR Exemption Number** Automated Export System (AES) or Foreign Trade Statistical Regulation (FTSR).
        
    -   When shipping from Canada, select a **B13A Filing Option** to show shipment export declaration was filed:
        
        -   If this option is **Not Required**, leave the field empty
            
        -   **Manually Attached**, enter the 21-character transaction number
            
        -   **Filed Electronically**, enter the authorization code number
            
        -   **Summary Reporting**, enter the 7-character summary ID number
            
        
        Export declarations (B13A) are required for shipments of goods worth over $2000CAN from Canada to any country other than Canada, the U.S., Puerto Rico, or the U.S. Virgin Islands.
        
    -   When shipping from Canada, enter **B13A Statement Data** to show that a shipment export declaration has been submitted
        
    -   If another party is being billed for this order, select a **3rd Party Billing Type** option:
        
        -   **None Selected** bill the main account for this location. No third party is charged
            
        -   **Bill Third Party** bill the third party account on this page or the FedEx third party account
            
        -   **Bill Recipient** bill the customer's FedEx customer record account
            
        -   **Collect** from the third party
            
        -   To bill the shipping charges to a third party account, enter a **3rd Party Billing Account Number**
            
            The customer record third party account number appears in this field by default. If no customer third party account exists, the third party account on the Company Information is used
            
            To learn more, see [Shipping Integration and Third Party Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265784.html).
            
        -   **None Selected** - bills the main account for this location as entered at _Setup > Accounting > Shipping_. No third party is charged
            
    -   Enter the **3rd Party Billing Zip** code associated with the third party account
        
    -   Select the **3rd Party Billing Country** associated with the third party account
        
    -   Select the **Duty Payment Type** for FedEx international shipments:
        
        -   **None Selected** to bill your account for duty payment
            
        -   To bill the **Recipient**, when fulfilling an order, enter the recipient's FedEx account number on the **Shipping** subtab
            
        -   To bill a **Third Party**, when fulfilling an order, enter the account number to bill on the **Shipping** subtab
            
    -   Enter the **Duty Payment Account Number** for duty payment for the third party and recipient
        
    -   For dutiable International Express shipments, select a **Terms of Sale** option
        
        This does not apply to international document express shipments.
        
    -   If you selected Cost & Freight (CF) or Cost, Insurance, Freight (CIF) in the Terms of Sale field, enter a **Terms Freight Charge**. This charge is added to the total customs value amount
        
    -   If you selected Cost, Insurance, Freight (CIF) in the Terms of Sale field, enter a **Terms Insurance Charge**. This charge is added to the total customs value amount
        
    -   To request delivery beyond the delivery site, check the **Inside Delivery** box
        
    -   To request pickup from a position inside the location, check the **Inside Pickup** box
        
    -   For Ground Economy returns, select an **Ancillary Endorsement** option
        
    -   if the customer wants to pick up a package from a designated FedEx location instead of having it delivered, complete the **Hold At Location** section:
        
        -   To display the Hold At Location fields, check the **Hold at Location** box
            
        -   The editable **Contact Phone Number** associated with the shipping address is displayed
            
        -   To list the nearest FedEx locations to Ship To address providing Hold at Location services, click **Retrieve locations**
            
        -   Enter the **Hold at FedEx Location** where the customer can collect the package
            
6.  Click the **Packages** subtab , and then select the following options:
    
    -   Enter the **Weight** in pounds for this package
        
    -   If it used in your package, enter the **Dry Ice Weight** in pounds
        
    -   The FedEx **Package Tracking Number** automatically populates this field after you save this fulfillment
        
    -   If you use FedEx, select the **Carrier Packaging** type using. If using your own packaging, select **Your Packaging**
        
    -   If you selected Your Packaging in the Carrier Packaging field, in the **Your Packaging** field, select a package type.
        
        If these order items are associated with a package type on the item record, packages are already created and added to the bottom of this subtab.
        
        Complete the Dimension fields
        
        Note:
        
        If you use the Pick, Pack, and Ship feature and have set Picked as the default status for item fulfillments, packages are not automatically created, even if items have associated package types. To learn more, see [Setting Up Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230197.html)
        
    -   If you are using your own packaging for shipments between the U.S., Canada, and Mexico, select an **Admissibility Package Type**.
        
    -   If this package is greater than 60 inches on any side, check the **Non Standard Container** box
        
    -   If the package contains alcohol, check the **Alcohol** box
        
        Select Customer or Licensee as the **Alcohol Recipient Type**
        
    -   Check this box, if the package contains **Non-Hazardous Lithium Batteries**
        
    -   If this package is to be insured, check the **Declared Value** box and then enter the monetary value
        
    -   In the **Reference Information** field, enter any additional information used to identify this package
        
    -   To have FedEx monitor your high value, time critical, or temperature critical shipments, select a **Priority Alert** option
        
    -   If you selected FedEx Priority Alert or FedEx Priority Alert Plus™ enter a package **Content Description**
        
    -   To calculate shipping rates, in the **Dimensions (Your Packaging Only)** fields, enter the package **Length**, **Height**, and **Width** in inches
        
    -   To request payment of goods on delivery, check the **C.O.D. Amount** box and then enter the amount to be collected from the customer
        
        This is only available with FedEx Express and FedEx Ground shipments
        
        Note:
        
        Express shipment - COD amount is calculated at shipment level only (not per package)
        
        Ground shipment - mixing COD and non-COD packages is not permitted
        
    -   When accepting C.O.D payments from the customer, select the **C.O.D. Method** you want FedEx to accept
        
    -   For C.O.D. shipments, select a **Freight Charge Added to COD Amount** to add to the COD amount:
        
        -   For orders with one package, add a **Shipping Charge**
            
        -   For orders with one package, add a FedEx **COD Charge**
            
        -   For orders with one package, add a **Total Charge**. For example, shipping charge and declared value surcharge, fuel surcharge, handling charges and taxes
            
        -   For orders with multiple packages, add a **Order Charge Total**. For example, shipping charge and other package charges
            
        -   For use with multiple packages, add a **Order Charge Net** . For example, add shipping charge for all packages
            
    -   If not specified elsewhere, enter a **COD Other Charge**
        
    -   Select a **Delivery Confirmation** type. Select Signature Required if the customer needs to sign for the delivery. Not available with FedEx Express Saver.
        
    -   If you selected Signature Required for delivery confirmation, select the **FedEx Delivery Signature Options** when obtaining a signature: **Adult** requires someone at the address over 21, and **Indirect** requires someone at the address, someone at the neighboring address, or a signed doortag.
        
        -   **Direct Signature** FedEx will accept a signature from any person at the delivery address
            
            Direct signature is the only permitted option for Canadian account
            
        -   **Indirect Signature** FedEx will accept a signature a person at the delivery address or a neighboring address. Alternatively, the recipient can sign a door form to release the package without anyone present
            
        -   **Adult** FedEx will only accept a signature from a person at the delivery address who is over 21 years of age
            
        -   **Service Default** represents the default FedEx delivery type option
            
    -   If you selected Deliver Without Signature in the Delivery Confirmation field, enter the **Signature Release** authorization number
        
    -   If you selected Signature Release in the Delivery Confirmation field, enter your FedEx **Authorization Number**
        
7.  Click **Add** after entering information about the package you are packing for this fulfillment. Repeat this step for all additional packages.
    
8.  Click **Save**.
    

### Related Topics:

-   [Getting Started with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268430.html)
-   [Printing USPS Shipping Labels and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1285080.html)
-   [Fulfilling Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1223349.html)
-   [Electronic Trade Documents (ETD) for International FedEx Shipments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1272548.html#bridgehead_N1272684)
-   [Shipping Dangerous Goods and Hazardous Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1269990.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
