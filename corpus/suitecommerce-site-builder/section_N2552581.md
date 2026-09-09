---
id: "section_N2552581"
type: "section"
title: "Resolving Permission Errors in Scriptable Cart"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Testing and Debugging Scriptable Cart > Resolving Permission Errors in Scriptable Cart"
parent: "section_N2550105"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2552581.html"
anchors: []
sha256: "3c4925effb2f444963414f43592625c990716c160dc494ad000bbccadd1bf2e7"
---

When you use custom records with Scriptable Cart, you might encounter permission errors when adding items in the shopping cart, or when attempting to check out. In most cases, careful review of the custom record you created, and the code in your script can resolve the problem.

For example, a common mistake is to code the script to use the current entity ID, and then test the script without logging in. Ensure that your script handles the case where the shopper is not logged in.

Use these guidelines to help resolve any permission errors you might see.

-   Check the custom record carefully:
    
    -   Verify that the Use Permissions box is marked.
        
    -   Clear the Include Name Field box on the Custom Record Type page for custom records that are created by your script.
        
    -   Clear the following boxes: Allow Attachments, Show Notes, Enable Mail Merge.
        
    -   On the Permissions subtab, set Level to Full for the following roles: Administrator, Customer Center, Shopper.
        
-   Review your script to verify that the record type ID you reference in your script matches the record type ID on the custom record in NetSuite.
    
-   Verify that the column IDs you reference in your script match the column IDs on the custom record in NetSuite.
    
-   Verify that you are correctly handling the true or false value returned in validation scripts. You must return either a true or false value in every case.
    
-   Ensure that you use the correct search operators when creating a search filter for custom records in your script.
    
    For example, you may need to use 'anyOf' instead of 'equals.' Note that the type of column you are searching may only support a specific set of search filters. For more information, see [SuiteScript 1.0 Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7151939532.html).
    

If you are still observing permission errors, try simplifying the script to its most basic components. Wrap each call in a try-catch statement, and then log any errors. See also, [Scriptable Cart FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553295.html).

### Related Topics

-   [Testing Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2550200.html)
-   [Debugging Your Shopping Cart Scripts Using Firebug](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2552787.html)
-   [Debugging Your Scriptable Cart with SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553048.html)
-   [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
