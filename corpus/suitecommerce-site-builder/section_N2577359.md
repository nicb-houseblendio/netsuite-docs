---
id: "section_N2577359"
type: "section"
title: "Customizing Login and Logout"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Setting Up Your Site Builder Site > Customizing Registration for Your Site Builder Web Store > Customizing Login and Logout"
parent: "section_N2576937"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577359.html"
anchors: ["bridgehead_N2577380", "procedure_N2577392", "bridgehead_N2577448", "procedure_N2577460"]
sha256: "c1cf7d7177b87decb893fb9d853902b6d96d50f1a8f11c204d637b24cde794ae"
---

You can display your company branding on a custom login page that you create for your employees, customers and partners. For more information about creating a secure hosted login page to NetSuite, see [Displaying Login Fields on Your Web Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577156.html). Also, you can further establish your company branding when members of your organization log out by specifying a custom logout landing page.

## Customizing Login {#bridgehead_N2577380}

When someone attempts to login with the wrong password or email, you can display an error on your hosted login page. This lets you maintain consistent company branding on the login page, instead of redirecting to a generic NetSuite branded error page.

#### To display an error on your custom hosted login page: {#procedure_N2577392}

1.  Add an error redirect hidden field to the login form in your hosted HTML page, for example:
    
                    `<form method="post" input type="hidden" name="errorredirect" value="/myloginpage.html"...` 
                  
    
2.  Add JavaScript, in the header of your login page, configured to read and display the error message.
    
3.  Upload your custom HTML page to the File Cabinet.
    
4.  Publish the secure URL of the hosted page to the people who use that page for login. The secure URL begins with https://. You can find the secure URL for your hosted page by clicking **Edit** next to the file record in the file cabinet
    

Now, when someone attempts to log in on your hosted page and fails, an error indicating the problem displays on your login page.

## Customizing Logout {#bridgehead_N2577448}

You can connect your company website's look and feel with the NetSuite application by specifying a landing page when employees, customers or partners log out.

#### To specify a landing page for logout: {#procedure_N2577460}

1.  Go to Setup > Company > General Preferences.
    
2.  Click the **Centers** subtab to select the appropriate center.
    
3.  Enter the URL for the **Log Out Landing Page**.
    

When employees, customers or partners click the Log Out link in the upper left of the NetSuite page, they are redirected to the custom HTML page you specified above.

### Related Topics

-   [Secure Login Access to Your NetSuite Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577046.html)
-   [Displaying Login Fields on Your Web Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577156.html)
-   [Registration-Free Shopping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577575.html)
-   [Restricting Access to Your Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577753.html)
-   [Customizing the Website Registration Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2578016.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
