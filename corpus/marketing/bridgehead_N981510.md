---
id: "bridgehead_N981510"
type: "bridgehead"
title: "Passing Parameters from Third Party Sites"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Capturing Leads > Passing Parameters Through URLs > Passing Parameters from Third Party Sites"
parent: "section_N979468"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N981510.html"
anchors: []
sha256: "7c8ca8e3e5a804edf200d5e6547c5c2418bbce96d3e8a09315d4addfc385ed93"
---

If NetSuite doesn't host your site, you'll need to add JavaScript to your web pages. This lets you pass parameters to any online customer forms you link to.

The following JavaScript code must be placed at the bottom of each page in your website. It should not be placed inside any HTML tags and should be the last code before the **</body>** tag.

          `<script type="text/javascript"> <!-- function getNS_url_param( name ){  name = name.replace(/[\[]/,"\\\[").replace(/[\]]/,"\\\]");   var regexS = "[\\?&]"+name+"=([^&#]*)";   var regex = new RegExp( regexS );   var results = regex.exec( window.location.href );   if( results == null )     return "";   else     return results[1]; } function trackNSParams() { var name = 'leadsource'; var value = getNS_url_param(name); if (value != null && value.length > 0)    document.cookie = name+"="+value+"; path=/"; } function appendNSParams(url) { var nameEQ = "leadsource="; var ca = document.cookie.split(';'); for(var i=0;i < ca.length;i++) { var c = ca[i]; while (c.charAt(0)==' ') c = c.substring(1,c.length); if (c.indexOf(nameEQ) == 0 )        url = url + '&' + nameEQ + c.substring(nameEQ.length,c.length); } return url; } // --> trackNSParams(); </script>` 
        

Then apply the following format to any links to online forms from your site (for example, Contact Us links):

          `<a href='#' onclick='document.location.href=appendNSParams(Publishable Form URL)'>Contact Us </a>` 
        

Paste the publishable form URL for the online customer form between the parentheses. For example:

          `<a href='#' onclick='document.location.href=appendNSParams(https://forms.netsuite.com/app/site/crm/externalleadpage.nl?compid=1234567&formid=3&h=ed62a43be13c70de335b)'>Contact Us </a>` 
        

When you copy and paste the form URL, make sure the single and double quotes are correct. If needed, you might have to retype the quotes.

For more information about URL Parameters, see [Tips for Passing Parameters Through URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N981583.html) and [Website URL Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611157.html)

### Related Topics

-   [Online Customer Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976289.html)
-   [Creating an Online Customer Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976686.html)
-   [Custom Field Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N981425.html)
-   [Tips for Passing Parameters Through URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N981583.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
