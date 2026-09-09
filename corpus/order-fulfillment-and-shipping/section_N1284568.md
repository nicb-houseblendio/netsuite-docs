---
id: "section_N1284568"
type: "section"
title: "Fulfilling Orders with USPS/Endicia Integration"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > U.S. Postal Service/Endicia > Fulfilling Orders with USPS/Endicia Integration"
parent: "section_N1283121"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1284568.html"
anchors: ["bridgehead_1478593243"]
sha256: "5cb6f254c44155ab935d4ce2e0e24ef41836e2a8519832e52fa408fdf045c473"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

#### To fulfill a USPS/Endica integration order:

1.  Enable the Shipping Label Integration feature:
    
    1.  Go to _Setup > Company > Enable Features_.
        
    2.  Click the **Transactions** subtab.
        
    3.  In the **Shipping & Receiving** section, check the **Shipping Label Integration** box.
        
    4.  Click **Save**.
        
2.  Ship the order with a USPS-integrated shipping item.
    
3.  Fulfill orders with USPS integration at _Transactions > Sales > Fulfill Orders_.
    
4.  Click the item you want to fulfill.
    
5.  Click the **Shipping** subtab:
    
    1.  Verify the shipping and address.
        
        Important:
        
        If you're shipping to Armed Forces Americas, Armed Forces Europe, or Armed Forces Pacific, the shipping address needs to follow a specific format for customs. Make sure you enter at least two letters in the City field. The Addressee field should have at least two letters, a space, and then at least two more letters. For example, John Wolfe.
        
    2.  Click the **Integrated Shipping Label** box.
        
    3.  Click **Save**.
        
6.  Click the **Carrier** subtab. Verify the following:
    
    -   To ship the package today, leave the **Future Ship Date** field empty.
        
        Otherwise, enter the date that you want to appear on the shipping label. You can enter a date up to seven days in the future.
        
    -   **Send Email Notification** - Check this box to notify the recipient that you are sending the package. For Express Mail labels, an email notification will be sent to this address with the Express Mail tracking number.
        
    -   The recipient **Email Address** is displayed.
        
    -   To indicate the package can be scheduled for weekend delivery, check the **Weekend Delivery** box.
        
    -   To ndicate the package can be scheduled for delivery on a holiday, check the **Holiday Delivery** box.
        
    -   To indicate this package is being sent by certified mail, check the **Certified Mail** box.
        
7.  Click the **Packages** subtab:
    
    -   Enter the total package **Weight** in pounds.
        
    -   Enter a **Package Contents Description**.
        
    -   After you save the fulfillment, the USPS **Package Tracking Number** is displayed.
        
    -   Select a **Carrier Packaging** option.
        
    -   To insure the package, check the **Insured Value** box and then enter the amount paid.
        
    -   **Reference #1, Reference #2** display the preference you set in _Setup > Accounting > Shipping_. If you did not select a preference, you can enter notes in these fields that will display on the shipping label.
        
    -   Select a **Package Confirmation** option for confirmation of delivery.
        
        The following options can result in additional charges from USPS:
        
        -   **Signature Confirmation™** - Requires a signature from the person who accepts your package. Get confirmation of delivery including date, time and location by using the Track & Confirm service online at www.usps.com, or by phone: 1-800-222-1811.
            
            You can add Signature Confirmation to the following: First-Class Mail Parcels, Priority Mail, Parcel Post, Media Mail and Library Mail.
            
        -   **Delivery Confirmation™** - Gives you the date, zip code and time your package was delivered. If delivery was attempted, you get the date and time of attempted delivery. You can access this information with the Track & Confirm service online at www.usps.com, or by phone: 1-800-222-1811.
            

Click Add/Edit after entering information about the package you are packing for this fulfillment. If you have more than one package for this order, you can enter information for the second package, and then click Add/Edit. Each package is saved on the fulfillment record.

## Package information disclosure when shipping with USPS/Endicia {#bridgehead_1478593243}

When Endicia (USPS) is selected as the shipping method, the following information is provided to Endicia when the shipping request is submitted.

| **Package information** | Packaging type, dimensions and weight |
| --- | --- |
| **Contents Value** | Total value of items in consignment |
| **Sales Order Number** | NetSuite-generated sales order no. |
| **Endicia account information** | Account ID and password |
| **Sender information** | Company contact name Company name Address information/Return address information (street, ZIP, city, state, country) Phone contact |
| **Consignee Information** | Company contact name Company name Address information (street, ZIP, city, state, country) Phone contact |

Note:

For international shipments, USPS requires specific information about the package contents. On the item record, you must enter information into the following fields for international shipping purposes: Sales Description, Country of Manufacture, Weight. If this information does not exist on the item record, then you will not be able to successfully submit the fulfillment.

### Related Topics:

-   [Fulfilling Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1223349.html)
-   [Printing USPS Shipping Labels and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1285080.html)
-   [United States Postal Service (USPS) Services through Endicia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1283121.html#bridgehead_N1283130)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
