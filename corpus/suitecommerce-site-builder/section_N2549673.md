---
id: "section_N2549673"
type: "section"
title: "Custom Error Messages for ValidateLine Events"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Custom Error Messages for ValidateLine Events"
parent: "chapter_N2545000"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549673.html"
anchors: ["procedure_N2549715"]
sha256: "cbfd0d75c14840ed2a9f67a5da1a54c387aa91e1320bcf0e4a4fb30260d3a9d7"
---

When shoppers on your site generate an error in a `validateLine` event, you can customize the error message on your site using customized website text, and a JavaScript alert.

#### To create a custom error message for validateLine events: {#procedure_N2549715}

1.  Add the logic for conditions that will trigger the error in your script attached to the scriptable template sales order form.
    
    Include the alert in your script. Note the code sample below:
    
                    `alert('Sorry-this item is on-hold due to safety issues.');    return false;` 
                  
    
2.  Go to _Commerce > Site Builder > Content > Customize Text_.
    
3.  Click the **Headings** subtab. Find the field containing the text, 'There is a problem with your order.'
    
4.  Edit the text by adding content for the error message you want to display on your site.
    
5.  Click **Save**.
    

### Related Topics

-   [SuiteScript for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2545233.html)
-   [Creating Customer-Facing Messages from Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2548158.html)
-   [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html)
-   [Testing and Debugging Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2550105.html)
-   [Scriptable Cart FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553295.html)
-   [Sample Scripts for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553996.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
