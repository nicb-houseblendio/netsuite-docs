---
id: "section_N2545233"
type: "section"
title: "SuiteScript for Scriptable Cart"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > SuiteScript for Scriptable Cart"
parent: "chapter_N2545000"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2545233.html"
anchors: ["bridgehead_N2545330"]
sha256: "f584f20ffc2f76d25046e0d70ab578c5701124b152d124867da7137260f49b95"
---

SuiteScript can only be executed from sales order forms on your website. This is because Web store shoppers are working exclusively with the sales order record type and the items sublist on the sales order when they add items to the shopping cart or enter a coupon code.

Note:

SuiteScript is not supported on registration forms.

Only a subset of the SuiteScript client event functions are available for use in Scriptable Cart. If you have not used SuiteScript before, read the topics, _User Event Scripts_ and _Client Scripts_ in the NetSuite Help Center.

Note:

You cannot use SuiteScript 2.0 user event scripts and client scripts at the same time for the Scriptable Cart. In most cases, it is better to use SuiteScript 1.0 for user event scripts and SuiteScript 2.0 for client event scripts; however, the reverse is also supported.

For code samples you can use to link events to functions in the shopping cart, see [Creating Custom Functions for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2545908.html).

For tips on using field change events in the Scriptable Cart, see [Working with Field Changed Client Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2546109.html).

See [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html) for a code sample you can use when changing values in ship method and shipping address fields.

For sample code you can use to display messages for customers, see [Creating Customer-Facing Messages from Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2548158.html).

To use the Scriptable Cart, you must first customize a sales order form by attaching your script. Next, go to _Commerce > Websites > Website List_, click Edit next to your website name, and select your customized forms. Then, customers on your website can use the sales order forms you customized for the shopping cart. For details, see [Getting Started with Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2545000.html#bridgehead_N2545032).

Note:

SuiteScript 2.1 client scripts are not currently supported in the Scriptable Cart. For more information about SuiteScript 2.1, see [SuiteScript 2.1](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_156042690639.html).

## Client Events Supported in Scriptable Cart {#bridgehead_N2545330}

The following table lists each client event type that you can use in Scriptable Cart. The functions executed on these events do not have to be called **recalc(), validateLine()**, **pageInit()**, and so on. However, it is best practice to indicate the client event type in the function name, for example: recalcCartItems(), validateLineOnItemAdd(), or pageInitOnLogin().

| 
Client Event/

Sample Custom Function Name



 | Parameters | Triggering Actions |
| --- | --- | --- |
| Field Changed Example: customFieldChanged(type,name, linenum) | _type_ : item (or blank). _name_ : the internal ID of the field that is changing. _linenum_ : item sublist line number. If _type_ is blank, then _linenum_ should also be blank. Note that line numbers start at 1, not 0. See also, [Working with Field Changed Client Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2546109.html). | Event occurs when a field is changed by the shopper or by another client call. Example actions:

-   when a shopper changes the Address field, the 'fieldChanged' event occurs and additional logic in the script is processed
-   when there is a change to the Coupon Code field, the 'fieldChanged' event occurs and additional logic in the script is processed

 |
| Page Init Example: customPageInit(type) | _type_ : create In the context of the web store, the value for this parameter must be create. | Event occurs when a shopper logs in to the web store. |
| postSourcing Example: postSourcing(type,name) | _type_ : the sublist internal ID _name_ : the field internal ID | Event occurs following a field change after all the field's child field values are sourced from the server. Enables fieldChange style functionality to occur after all dependent field values have been set. For more information, see [Working with Field Changed Client Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2546109.html). |
| Recalc Example: customRecalc(type, action) | _type_ : item _action_ : commit, batchcommit, insert, or remove | Event occurs after the shopping cart changes. Example actions:

-   when a shopper adds an item to the shopping cart, the 'recalc' event is triggered, and the order amount is recalculated (commit)
-   when a shopper deletes an item from the cart, the 'recalc' event is triggered and the order amount is recalculated (remove)
-   when the quantity of an item changes in the shopping cart, the 'recalc' event is triggered and the order subtotal is recalculated (commit)

 |
| saveRecord |  | Event occurs when the submit button is pressed but prior to the form being submitted. You should always return a Boolean value, either true or false, from a saveRecord event. A return value of false suppresses submission of the form. The function associated with the 'saveReacord' event should return false to reject the shopper's attempt to submit the order. Example actions:

-   shopper submits the order, and a 'saveRecord' event occurs. This event triggers a script that throws an alert notifying the shopper additional information is needed for the order to be submitted.
-   shopper submits the order, and a 'saveRecord' event occurs. This event triggers a script that shows an alert so the shopper can confirm she wants to submit the order.

 |
| Validate Line Example: customValidateLine(item) | _type_ : item Note: This client event function must return a value of true or false. | Event occurs prior to another item being added to the shopping cart. For example: Return false to reject the addition of the new item. |

### Related Topics

-   [Creating Custom Functions for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2545908.html)
-   [Working with Field Changed Client Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2546109.html)
-   [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html)
-   [Testing and Debugging Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2550105.html)
-   [Sample Scripts for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553996.html)
-   [Scriptable Cart FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553295.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
