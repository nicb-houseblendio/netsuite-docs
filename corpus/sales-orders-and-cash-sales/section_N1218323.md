---
id: "section_N1218323"
type: "section"
title: "Getting Credit Card Authorization Automatically on Sales Orders"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Sales Orders > Creating Sales Orders > Getting Credit Card Authorization Automatically on Sales Orders"
parent: "section_N1216500"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1218323.html"
anchors: []
sha256: "d1460cf2150bb0c13190cbdf710adb2660f815bafcf65e9796a308b02eb54617"
---

You can customize sales orders to automatically get credit card authorization. This saves you from having to check the Get Authorization box on each order.

To customize sales order forms, go to _Setup > Customization > Transaction Forms_ (Administrator) and click **Customize** next to the standard sales order form. On the custom form, click the **Screen Fields** subtab and then click **Payment**. Check the boxes as follows:

-   Check the **Get Authorization** box to use the Get Authorization box on the form.
    
-   Check the **Show** box to display the field on the form. Clear the Show box to hide the field.
    
-   Check the **Default Checked** box to set the default value for the Get Authorization box. Now, the box is checked by default, unless you clear it.
    

If the Default Checked box is checked but not the Show box, orders with credit card information will still try to authorize the charge when saved.

If the Display Type field is set to Inline Text, then the Get Authorization field shows Yes or No, depending on your setting for Default Checked.

When you're done customizing and save an order with credit card information, the gateway automatically authorizes the card. If authorization fails, you're notified and need to update the payment information before resubmitting.

Please note the following about using the Get Authorization box:

-   If you set both Get Authorization and Credit Card Approved to **Default Checked**, Get Authorization takes priority. In this case, only Get Authorization will be checked on the form.
    
-   You'll only see Get Authorization when editing a transaction, not when viewing it.
    
-   If both boxes are checked but no credit card number is entered, Get Authorization will be unchecked when you edit the order later.
    
-   For Web Store orders, the Require Authorization preference overrides the Default Checked setting.
    

### Related Topics

-   [Creating Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1216500.html)
-   [Adding Items on a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4588373194.html)
-   [Applying a Promotion on a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160312998339.html)
-   [Applying a Discount on a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160312998983.html)
-   [Entering Accounting information about a Sales Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4587464246.html)
-   [Assigning Locations Automatically in a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4558169323.html)
-   [Creating Store Pickup Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4835438208.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
