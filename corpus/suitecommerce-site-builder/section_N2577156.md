---
id: "section_N2577156"
type: "section"
title: "Displaying Login Fields on Your Web Page"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Setting Up Your Site Builder Site > Customizing Registration for Your Site Builder Web Store > Displaying Login Fields on Your Web Page"
parent: "section_N2576937"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577156.html"
anchors: ["procedure_4706929897"]
sha256: "77784d8017b331ba030bfd3dbfb2b9e1caf70bbc9a92e9cda628daacf8b67641"
---

You can operate a website hosted by NetSuite and still allow your users to log in to your NetSuite account. You can also create a custom login page that displays your company's branding on the page used to log in to your NetSuite account.

To display your company's branding on the NetSuite account login page, you must create a custom login page that is **hosted in the NetSuite File Cabinet**, then display a link to it on a different page on your website.

Your custom login page, and any images displayed on it, must be uploaded to the images folder in the file cabinet at Documents > Files > Images. Also, you must use the secure URL displayed on the file record in any tags you use to display content on your login page.

The security team at NetSuite does not allow the practice of presenting login fields to your NetSuite account in an iFrame on your web page. The following procedure has been approved by the security team at NetSuite to provide login access to your NetSuite account.

The following procedure describes how to create custom login pages. If you are creating a custom login page for Customer Center roles, you must know your account ID to complete this procedure. The variable in the following code example is <ACCOUNT\_ID>).

To locate your account ID, go to Setup > Company > Company Information. The account ID field is located near the bottom of the right column.

#### To create a custom login page to your NetSuite account: {#procedure_4706929897}

1.  Create a custom login page in HTML, using the code below to display the NetSuite account login fields. Save the HTML file to your hard drive.
    
    -   If you are creating a custom login page for non-Customer Center roles, you could, for example, name the file `NSlogin.html`. You do not have to modify the code shown below if you are creating a non-Customer Center login page.
        
    -   If you are creating a login page for Customer Center roles, you could name the file, for example, `NSprivatelogin.html`. You must modify two lines in the sample. In each line you modify, replace the variable <ACCOUNT\_ID> with your account ID.
        
        -   Modify the first line (the post action link) as shown:
            
            `<form method="post" action="/app/login/secure/privatelogin.nl">`
            
        -   Modify the href line for the Forgot your password link as shown:
            
            `<href="https://docs.oracle.com/app/login/preparepwdreset.nl?private=t">`
            
    
    Note:
    
    The code only represents the basic required fields for login to your NetSuite account. You can add content to this file, but you must use a secure URL to refer to any additional files.
    
                    `<!--The post action link below is for a non-Customer Center login page--> <form method="post" action="app/login/secure/enterpriselogin.nl"> <!--For a Customer Center login page, modify the post action link as specified in step 1.-->    <table border="0" cellspacing="0" cellpadding="3">       <tr>          <td>             Email address:<input name="email" size="30">          </td>       </tr>       <tr>          <td>             Password:<input name="password" size="30" type="password">          </td>       </tr>       <tr>          <td>             <!--The href link below is for a non-Customer Center login page-->             <a href="https://docs.oracle.com/app/login/preparepwdreset.nl">Forgot your password?</a>             <!--For Customer Center login page, modify the href link as specified in step 1.-->          </td>       </tr>       <tr>          <td>             <input type="submit" name="submitter" value="Login" >          </td>       </tr>    </table> </form>` 
                  
    
2.  Go to the Images folder in the NetSuite File Cabinet (Documents > Files > Images).
    
3.  Click **Add File**, and then select the appropriate HTML file for the custom login page that you created in step 1.
    
4.  Click **Open**. The HTML file for your custom login page is uploaded to the file cabinet. You can also add any additional files you want to use for content on your custom login page to this folder.
    
5.  Click **Edit** next to the file you have uploaded. Ensure that the "Available without login" box is selected.
    
6.  Determine the secure URL for your custom login page. You will use the secure URL later to display the link to your custom login page.
    
    1.  Go to the Images folder in the NetSuite File Cabinet (Documents > Files > Images).
        
    2.  Click **Edit** next to the HTML file for your custom login page.
        
    3.  Copy the NetSuite URL that starts with `https://<accountID>.app.`... You will use this URL to create a link to your login page.
        
7.  Reference your custom login page from your website. You can now link to your custom login page from any external source by adding an `href` that uses the secure URL you copied in step 5.c.
    
    For example:
    
                    `<a href="https:<accountID>.app.netsuite.com/....>Login Here</a>` 
                  
    
    Do not copy the example! Use the URL you copied in step 5.c. in your `href`.
    
    Important:
    
    The HTML file for your custom login page you created in step 1 **must** be hosted in the NetSuite File Cabinet. The external source hosting the link **does not** have to be in the NetSuite File Cabinet.
    

When visitors click the link to your custom login page, they can enter their email and password on the page you created that displays your company's branding.

### Related Topics

-   [Secure Login Access to Your NetSuite Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577046.html)
-   [Customizing Login and Logout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577359.html)
-   [Registration-Free Shopping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577575.html)
-   [Restricting Access to Your Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577753.html)
-   [Customizing the Website Registration Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2578016.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
