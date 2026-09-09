---
id: "section_N2540093"
type: "section"
title: "Integrating with PayPal Express"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Integration with Third-Party Checkout Providers > Integrating with PayPal Express"
parent: "section_N2539882"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2540093.html"
anchors: ["bridgehead_N2540220", "bridgehead_N2540238"]
sha256: "91a13a4a60774e24803cfcdbbf844abb2df9238f265c147a39d96bdbb0feb9be"
---

To integrate SSP application checkout with PayPal Express, do the following for the View Cart and Proceed to Checkout touch points:

-   Get the [checkoutsettings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2516589.html) JSON object by calling `nlapiGetWebContainer()`.`getShoppingSession()`.`getSiteSettings()`.
    
-   Ensure that the checkout.paypalexpress.available field is set to T in the `checkoutsettings` object.
    
-   Get the image URL for PayPal Express from the checkout.paypalexpress.imageurl field in the `checkoutsettings` object
    
-   Add the Paypal Express Checkout button to your touch point .ssp file and provide a handler, in an .ss file, that calls the `proceedToCheckout()` method on the shopping session, to integrate with the PayPal Express checkout flow.
    
    Values for checkoutsettings fields should be passed as parameters for this method. You can set values for the following fields to customize the default PayPal Express checkout flow:
    
    -   **type** - set to paypalexpress
        
    -   **cancelurl** - the URL of redirect page when Cancel link is clicked at PayPal site
        
    -   **continueurl** - the URL for redirect page when Continue link is clicked at PayPal site
        
    -   **createorder** - if value is set to T, Backend submits the current shopping order when Continue link is clicked; default is F
        

Besides the .ss file, integration with PayPal Express requires client-side code to display PayPal Express information in the user interface. For code examples, see the following:

-   [Sample .ss File for PayPal Express Integration](#bridgehead_N2540220)
    
-   [Sample for Displaying PayPal Express Information](#bridgehead_N2540238)
    

Note:

Integration with third-party checkout providers is not available for SSP applications written in Suitescript 2.0. For more information about SuiteScript 1.0, see [SuiteScript 1.0 Guide.](https://system.netsuite.com/app/help/helpcenter.nl?fid=SuiteScript10.pdf)

## Sample .ss File for PayPal Express Integration {#bridgehead_N2540220}

The following code is in a samplePaypalCheckout.ss file:

          `function service(request,response) {     var returnval = null;       try     {           var shoppingSession = nlapiGetWebContainer().getShoppingSession();         var siteSetting = shoppingSession.getSiteSettings(['touchpoints']);           var viewcart = siteSetting.touchpoints.viewcart;         var homeurl = siteSetting.touchpoints.home;           var checkoutSetting = {type: 'paypalexpress', continueurl: homeurl, cancelurl : viewcart};           nlapiGetWebContainer().getShoppingSession().proceedToCheckout(checkoutSetting);     }     catch (e)     {         var nle = nlapiCreateError(e);         returnval = {status : 'error', reasoncode : nle.getCode(), message : nle.getDetails()};           response.writeLine(JSON.stringify(returnval));     } }` 
        

## Sample for Displaying PayPal Express Information {#bridgehead_N2540238}

You can use the following code for PayPal Express integration. Note how the getAbsoluteURL(domain, path) method is used for the Shopping Session object. You'll need the absolute path to avoid errors with cross-domain links (links that go between shopping and checkout domains).

          `<table border=0> <% var checkoutSettings = nlapiGetWebContainer().getShoppingSession().getSiteSettings(['checkout']); var paypalUrl = nlapiGetWebContainer().getShoppingSession().getAbsoluteUrl("checkout", "samplePaypalCheckout.ss"); var proceedToCheckoutUrl = nlapiGetWebContainer().getShoppingSession().getAbsoluteUrl("checkout", "sampleCheckout.ss"); <tr>   <td>     <form name='checkoutform' action='<%=proceedToCheckoutUrl%>' method='post'>       <input type="submit" name="placeorder" value="Proceed To Checkout"/>     </form>   </td>   <td> </td>   <td >     <form name='paypalform' action='<%=paypalUrl%>' method='post'>       <input type='image' src='<%=checkoutSettings.checkout.paypalexpress.imageurl%>'/>     </form>   </td>   </tr> </table>` 
        

          `function service(request,response) {    var returnval = null;      try    {         var shoppingSession = nlapiGetWebContainer().getShoppingSession();       var siteSetting = shoppingSession.getSiteSettings(['touchpoints']);         var viewcart = siteSetting.touchpoints.viewcart;       var homeurl = siteSetting.touchpoints.home;         var checkoutSetting = {type: 'paypalexpress', continueurl: homeurl, cancelurl : viewcart};         nlapiGetWebContainer().getShoppingSession().proceedToCheckout(checkoutSetting);    }    catch (e)    {       var nle = nlapiCreateError(e);       returnval = {status : 'error', reasoncode : nle.getCode(), message : nle.getDetails()};         response.writeLine(JSON.stringify(returnval));    } }` 
        

### Related Topics

-   [Integrating with 3D Secure (SCA Elbrus and Earlier)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2544266.html)
-   [Integration with Third-Party Checkout Providers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2539882.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
