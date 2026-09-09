---
id: "section_N1279306"
type: "section"
title: "Fulfilling Orders with UPS"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > UPS > Fulfilling Orders with UPS"
parent: "section_N1274266"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1279306.html"
anchors: []
sha256: "d25966b516b7cf1e7775fc771a5297262f2025ffec6bb25710613abe1d526e42"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

When fulfilling a UPS-integrated shipping order, and have enabled Shipping Label Integration and selected UPS as the default shipping carrier, additional options are available.

Warning:

These options may result in extra charges from UPS. To learn more, see [www.ups.com](http://www.ups.com).

#### To fulfill an order using UPS integration:

1.  Enable the Shipping Label Integration feature:
    
    1.  Go to _Setup > Company > Enable Features_.
        
    2.  Click the **Transactions** subtab.
        
    3.  In the **Shipping & Receiving** section, check the **Shipping Label Integration** box.
        
    4.  Click **Save**.
        
2.  Ship the order with a UPS-integrated shipping item.
    
3.  Fulfill orders with UPS integration at _Transactions > Sales > Fulfill Orders_.
    
4.  Click the **Shipping** subtab:
    
    1.  Verify the shipping and address
        
    2.  Click the **Integrated Shipping Label** box.
        
    3.  Click **Save**.
        
5.  Click the **Carrier** subtab, and then select the following options:
    
    -   To deliver this UPS shipment on a Saturday, check the **Saturday Service** box. Extra charges may apply.
        
    -   To alert the recipient when the package is shipped, check the **Ship Notification Email Addresses** box.
        
        Enter a contact email address. You can enter a second e-mail address to be copied on this notification.
        
    -   Enter a **Shipper Email Address**.
        
        UPS uses this address to send shipment notifications and resolve customs issues for international shipments.
        
    -   In case messages to the above email addresses are undeliverable, check **If Notifications are Undeliverable, please email** box
        
        Enter an e-mail address to send shipment notification
        
        Back-up notification e-mail can result in extra charges from UPS. For more information, visit www.ups.com
        
    -   Enter an **Email Message** to display in the notification email
        
    -   To bill the shipping charges to an account other than your own, enter the UPS account number in the **3rd Party Billing Account Number**. Be sure to select Bill Third Party in the 3rd Party Billing Type field.
        
        For example, your company's production account, a vendor account, or the customer account number.
        
    -   Enter the **3rd Party Billing Zip** code associated with the third party account.
        
    -   Select the **3rd Party Billing Country** associated with the third party account.
        
    -   Select the **3rd Party Billing Type** to use for this account:
        
        -   To bill the location main account, select **None Selected**. No third party is charged.
            
        -   To bill the specified third party or UPS third party account, select **Third Party Billing**.
            
        -   To bill the customer UPS account , select **Consignee Billing**.
            
6.  Click **Save**.
    
7.  Click the **Packages** subtab , and then select the following options:
    
    -   This field displays the **Total Package Weight** of all packages for this order.
        
    -   Enter the total package **Weight** in pounds (lbs).
        
        UPS has special guidelines for packages over 70 lbs. To learn more, see [www.ups.com](http://www.ups.com).
        
    -   For customs purposes, enter a **Package Contacts Description**.
        
    -   Enter a **Package Tracking Number**.
        
        If you use UPS integrated shipping, a tracking number is displayed after you fulfill the order.
        
    -   Select a UPS **Carrier Packaging** type. If you are using your own packaging, select Your Packaging.
        
        If you select Your Packaging, enter the package Dimensions are required.
        
    -   If this package is to be insured, check the **Declared Value** box.
        
        Enter the value in U.S. dollars
        
    -   Enter additional **Reference Numbers** you are using to identify this package.
        
    -   If you selected Your Packaging in the **Dimensions** (Your Packaging Only):
        
        -   Measure the longest side of the package, and then enter the **Length** in inches.
            
            UPS does not ship packages over 108 in. long.
            
        -   Enter the package **Width** in inches.
            
        -   Enter the package **Height** in inches.
            
    -   If the total package size exceeds 130 inches (330 cm), the **Large Package** box is automatically checked.
        
        An additional handling fee is not charged, but other additional fees apply.
        
    -   If other UPS charges apply, check the **Additional Handling** box. UPS charges additional handling for the following:
        
        -   any article encased in an outside shipping container made of metal or wood
            
        -   any cylindrical item, such as a barrel, drum or tire, that is not encased in a box
            
        -   any package with the longest side exceeding 60 inches or the second-longest side exceeding 30 inches
            
    -   If you are using UPS's Collect on Delivery service, check the **C.O.D Amount** box
        
        Enter the C.O.D. amount in US dollars (USD).
        
        **C.O.D. Amount** - The COD amount updates with additional surcharges when you click the Calculate button on the Shipping subtab on the Item Fulfillment. You can re-enter the C.O.D. amount before saving the fulfillment if you want.
        
    -   Select a customer **C.O.D. Method** payment.
        
    -   If you are using delivery confirmation from UPS, select a **Delivery Confirmation** type.
        
        Delivery confirmation results in extra charges from UPS.
        
8.  Click **Add** after entering information about the package you are packing for this fulfillment. Repeat this step for all additional packages.
    
9.  Click **Save**.
    
10.  Click the **International** subtab.
     
     To set international options, **Enable International Shipping**:
     
     1.  Go to _Setup > Accounting > Shipping_
         
     2.  Click the **Preferences** subtab.
         
     3.  In the **Carrier Basics** section, check the International Shipping box.
         
     4.  Click **Save**.
         
11.  Select the following options:
     
     -   if this is a related party transaction, check the **Parties to Transaction** box.
         
         A related party transaction is between a U.S Principal Party in Interest (USPPI) and a foreign consignee (a parent company or sister company) where there is at least 10% ownership of each by the same U.S. or foreign person or business.
         
     -   For the merchandise being shipped, select an **Export Type**:
         
         -   **Domestic Exports** - merchandise is grown, produced or manufactured in the U.S., including imported merchandise that has been enhanced in value or changed in form
             
         -   **Foreign Exports** - merchandise has entered the U.S. and is being re-exported in the same condition
             
         -   **Foreign Military Sales** - merchandise is being sold under the Foreign Military Sales program
             
     -   Select a shipment **Reason for Export**.
         
     -   Enter a merchandise export **Method of Transport**. For example, vessel, air, rail, or truck.
         
     -   For vessel, rail, and truck shipments, enter the 4-digit Standard Carrier Alpha Code (SCAC) **Carrier Identification Code**.
         
         Alternatively, enter the 2-3 character International Air Transport Association (IATA) Code for the air shipments carrier.
         
         To learn more, see [www. census.gov/foreign-trade](http://www.census.gov/foreign-trade).
         
     -   When the export transaction is used as proof of export for import transactions, enter the import **Entry Number**. For example, In-Bond, Temporary Import Bond, or Drawback's.
         
     -   To indicate whether the shipment is being transported under bond, enter a 2-character **In Bond Code**. These codes are listed in Part IV of Appendix C of the Foreign Trade Statistics Regulations (FTSR) (15 CFR Part 30).
         
         To learn more, see [www.census.gov/foreign-trade](http://www.census.gov/foreign-trade).
         
     -   If the foreign principal party in interest authorizes a U.S. forwarding agent or other agent to export the merchandise out of the U.S., check the **Routed Export Transaction** box
         
     -   Iif you are operating under the authority of the Department of the Treasury, Office of Foreign Assets Control license, a Department of Justice DEA permit, or any other export license issued by a Federal government agency, enter the **License Number**.
         
     -   Enter the license number **License Date**.
         
     -   If you are operating under the authority of a license exception, select the **License Exception** scronym
         
     -   Enter the Export Control Classification Number **ECCN** for the following:
         
         -   exports authorized under a license or License Exception
             
         -   items being exported under the NLR provisions listed on the CCL with a reason for control other than anti-terrorism
             
     -   For the business receiving the shipment, enter the **Recipient Tax Identification Number**.
         
     -   For the blanket period of up to one year that the applicable North American Free Trade Agreement (NAFTA) Certificate of Origin is in effect, enter the **Blanket Period Start Date**.
         
     -   Enter the NAFTA Certificate of Origin **Blanket Period End Date**.
         
12.  Click **Save**.
     

Note:

UPS only accepts packages up to 150 pounds. Packages weighing more than 150 pounds are broken into multiple shipments for calculating UPS Real-Time rate charges. For example, a shipment of 400 pounds is charged as two 150-pound shipments and one 100-pound shipment. Visit the [UPS Web site](http://www.ups.com) to learn more about UPS size and weight limitations.

When using the UPS Developer Kit, NetSuite displays the UPS Trademark and accompanying disclaimer\* on each shipping screen and shipment notification viewed by your customer. These elements are permanent and cannot be deleted or altered.

\* UPS, UPS & Shield Design, and UNITED PARCEL SERVICE are registered trademarks of United Parcel Service of America, Inc.

### Related Topics:

-   [UPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278000.html)
-   [Voiding a UPS Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1282009.html)
-   [Printing USPS Shipping Labels and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1285080.html)
-   [Fulfilling Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1223349.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
