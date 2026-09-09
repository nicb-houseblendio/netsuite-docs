---
id: "section_N2545908"
type: "section"
title: "Creating Custom Functions for Scriptable Cart"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > SuiteScript for Scriptable Cart > Creating Custom Functions for Scriptable Cart"
parent: "section_N2545233"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2545908.html"
anchors: ["bridgehead_N2545931", "bridgehead_N2545947", "bridgehead_N2545962", "bridgehead_N2545978", "bridgehead_N2545997", "bridgehead_N2546014"]
sha256: "b018d33f2ffc1cdcd880a61d1502c2a7237c38aa5ce3789ccc61fb01adfa0bfd"
---

By creating custom functions, you can link events to functions that are only applicable to the shopping cart. Because your script is running against a sales order form, other events related to a sales order transaction also run along with the events you specify in your script for the shopping cart. This could adversely impact performance.

The main reason for creating custom functions is to filter out events that do not apply to the web store. Sample custom functions are listed below:

## function customInit(type) {#bridgehead_N2545931}

Use this custom function to call any functions related to login.

          `function customInit(type) {    //call any functions related to login here. }` 
        

## function customOnChange(type, name, linenum) {#bridgehead_N2545947}

Use this custom function to link to the FieldChanged event and filter out non-Web store events.

          `function customOnChange(type, name, linenum) {          if (name == 'promocode')          {    // call any functions that are triggered by promocode here         sample();   }` 
        

## function customRecalc(type, action) {#bridgehead_N2545962}

Use this custom function to link to the Recalc client event. In Scriptable Cart, the action can only be 'commit' or 'remove.' Note that only events related to items are applicable to Scriptable Cart.

          `function customRecalc(type, action) {             if (type == 'item')             {                         // call any functions related to recalc here                         sample1(action);                         sample2(action);             } }` 
        

## function customValidateLine(type) {#bridgehead_N2545978}

Use this custom function to link to the ValidateLine event. Note that all validations occur in the item list on the shopping cart page. For best results, filter out any events that are not executed against items.

The return value of each function called from customValidateLine must be tested. If any function returns false, processing must stop and return false.

          `function customValidateLine(type) {             if (type != 'item')             {                         return true;             }              if (!sample())             {                         return false;             }             if (!bar())             {                         return false;             }             // All validations passed, so return true             return true;` 
        

## function customBeforeSubmit() {#bridgehead_N2545997}

This custom function will execute before a sales order is saved. Scripts that include the beforeSubmit() gateway function must be attached to a script record of type User Event.

          `function customBeforeSubmit() {             return sample(); }` 
        

## function customAfterSubmit() {#bridgehead_N2546014}

This custom function will be run after a sales order is saved. Scripts that include the afterSubmit() gateway function must be attached to a script record of type User Event.

          `function customAfterSubmit() {             return sample(); }` 
        

Note:

You can combine the deployment for both the customBeforeSubmit() function and the customAfterSubmit() functions on the same script deployment record when necessary. For more information, see [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html).

### Related Topics

-   [Working with Field Changed Client Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2546109.html)
-   [SuiteScript for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2545233.html)
-   [Sample Scripts for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553996.html)
-   [Scriptable Cart FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553295.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
