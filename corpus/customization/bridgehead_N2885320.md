---
id: "bridgehead_N2885320"
type: "bridgehead"
title: "Creating an HTML Template Locally"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Records Overview > Creating Custom Record Types > Online Custom Record Forms > Creating HTML Templates for Online Custom Record Forms > Creating an HTML Template Locally"
parent: "section_N2885246"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2885320.html"
anchors: []
sha256: "b852cccb0cc292c1cac47c890899bbf243087006644226b31e51ed0ff17acef8"
---

When creating an online form template on your local machine, you can define how the fields are arranged, which fields to include on the form and the style of the page. Use standard HTML code to create the template as you would for any other HTML form and include the following elements:

-   <NLFORM> and </form> tags to define the beginning and end of the form.
    
-   Tags for each NetSuite field included on the form. For more information, see [Using NetSuite Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2885392.html).
    
-   An input tag that defines the button your customers use to submit the form.
    
                  `<input type="submit" value="Button Text">` 
                
    
    You can substitute text in the button by changing the value in the code. For example, if you want the text in the button to read Submit Form, the code would be:
    
                  `<input type="submit" value="Submit Form">` 
                
    

For example, the following HTML code is a representation of an acceptable form template:

          `<html> <head> </head> <body> <NLFORM> <p>Enter the name of your company: <NLNAME></p> <p>Enter an email address we can use to contact you: <NLCUSTRECORD1></p> <p><input type="submit" value="Submit Form"></p> </form> </body> </html>` 
        

Important:

The resulting file must include all tags, including <html>, <head> and <body> tags, to ensure that it's a valid HTML file recognizable by NetSuite.

### Related Topics

-   [Creating HTML Templates for Online Custom Record Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2885246.html)
-   [Using NetSuite Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2885392.html)
-   [Uploading an HTML Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2885453.html)
-   [Creating an HTML Form Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2885567.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
