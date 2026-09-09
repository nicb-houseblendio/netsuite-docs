---
id: "section_N1269731"
type: "section"
title: "FedEx Customer Returns"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > FedEx > FedEx Customer Returns"
parent: "section_N1267302"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1269731.html"
anchors: ["bridgehead_N1269828", "procedure_1547660096", "bridgehead_N1269870", "procedure_N1269884", "bridgehead_N1269944", "bridgehead_N1269957"]
sha256: "9cb73c251c4e29b858a13c6523cc8fa01256e60f12d74dd6750200dc39fc8708"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

Including customer return labels with FedEx shipments provides a convenient customer return solution. Customer return labels are only available with FedEx integration for domestic and international shipments.

To set up and use customer return labels with your FedEx integration, complete the following:

-   [Adding Return Addresses](#bridgehead_N1269828)
    
-   [Updating FedEx Shipping Items for Return Labels](#bridgehead_N1269870)
    
-   [Fulfilling Orders with FedEx Customer Return Labels](#bridgehead_N1269944)
    
-   [Processing FedEx Customer Returns](#bridgehead_N1269957)
    

## Adding Return Addresses {#bridgehead_N1269828}

For each site that accepts returns, verify that you have recorded a customer shipping address. You can add a return address at the location, subsidiary (OneWorld only), and company levels.

#### To add a return address for a location:

1.  Go to _Setup > Company > Locations_.
    
2.  Beside the location you want to update, click **Edit**.
    
3.  In the **Address** subtab, beside **Return Address**, click **Edit**.
    
4.  Complete the [To complete the return address form:](#procedure_1547660096) procedure.
    
    Click **Save**.
    

#### To add a return address for a subsidiary:

1.  Go to _Setup > Company > Subsidiaries_.
    
2.  Beside the subsidiary you want to update, click **Edit**.
    
3.  In the **Address** subtab, beside **Return Address**, click **Edit**.
    
4.  Complete the [To complete the return address form:](#procedure_1547660096) procedure.
    

#### To add a return address for a company:

1.  Go to _Setup > Company > Company Information_.
    
2.  Beside the company you want to update, click **Edit**.
    
3.  In the **Address** subtab, beside **Return Address**, click **Edit**.
    
4.  Complete the [To complete the return address form:](#procedure_1547660096) procedure.
    

#### To complete the return address form: {#procedure_1547660096}

1.  Enter the **Country** this address is located in.
    
2.  Enter the name of the person the shipment is addressed to in the **Attention** field.
    
    This is the name that appears on the shipping label.
    
3.  Enter the name of the entity that should appear on the shipping label in the **Addressee** field.
    
    This name appears on the shipping label under the Attention field.
    
4.  Enter the address **Phone** number.
    
5.  Enter the **Address** as it appears on forms. Enter up to 50 characters
    
    If this address is marked default for shipping or billing, it automatically populates employee, customer, partner, and vendor, addresses on forms.
    
6.  Enter the address **City**, **State**, and **Zip** code.
    
7.  Check the **Override** box to disable the free-form address text field so text is not displayed in the Address field.
    
8.  Click **OK**.
    

If a location has no return address, the subsidiary return address for a subsidiary is used, if provided. if not, the company return address for the company is used. If a return address for the location, subsidiary, or company is not provided, manually enter the return address for each item fulfillment.

The following diagram describes the return address process:

![Flowchart showing steps in the item fulfillment return address process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/OrderFulfillmentShipping/Workflow_ReturnAddressItemFulfillment.png)

## Updating FedEx Shipping Items for Return Labels {#bridgehead_N1269870}

You must update each FedEx shipping item that you provide customer return labels for. When the shipping item is used on an order, a customer return label prints when the shipping label prints.

#### To update FedEx shipping items for customer return labels: {#procedure_N1269884}

1.  Go to _Shipping > Lists > Shipping Items_.
    
2.  Click **Edit** for the FedEx shipping item you want to update.
    
3.  Check the **Return Label Integration** box and select a FedEx integrated shipping item from the list.
    
4.  **Save**.
    

## Fulfilling Orders with FedEx Customer Return Labels {#bridgehead_N1269944}

After you fulfill an integrated FedEx shipping order item enabled for return label integration, the return shipping label and shipping label are printed. Fulfill your order and then select Save and Print Label, or print shipping labels in bulk. The return tracking number and shipment tracking number are displayed on the order fulfillment page, cash sale page, and return authorization page.

## Processing FedEx Customer Returns {#bridgehead_N1269957}

When a customer returns an item using a FedEx return label, follow the [Customer Returns Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1303799.html). The return authorization displays the return tracking number generated for the original order.

To learn more, see [Entering a Linked Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1306234.html).

When processing FedEx International returns, you can select the return type. This helps the customs agent understand the reason for the return.

On the Item Fulfillment form **Shipping** subtab, when you select a FedEx International shipping method, you can also select Return Type values. If there is no option matching your reason for returning the item, select **Other** and then enter a reason in the **Return Type Description Field**. The Return Type field is only to be used with international orders. The value of the return type appears on the return label.

### Related Topics

-   [FedEx](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1267302.html)
-   [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html)
-   [Registering a FedEx Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1267302.html#bridgehead_N1267326)
-   [Getting Started with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268430.html)
-   [Customer Returns Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1303799.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
