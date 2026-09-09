---
id: "section_N2429074"
type: "section"
title: "Linking to Online Forms"
branch: "setting-up-case-management"
category: "support-management"
breadcrumb: "Support Management > Setting Up Case Management > Online Case Forms > Linking to Online Forms"
parent: "section_N2428291"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2429074.html"
anchors: []
sha256: "606f1d1ddf9df39af442817b991cb351689ecf938af34a7be40a80a9bfa8fb62"
---

You can link to an online form from your website, an email, or a template. Find the form URL on the External subtab of the form record. Use the Publishable Form URL when linking from an external website. Use the Internal Form URL when linking to a form from a NetSuite website or intranet site. Also use this URL when linking from the Partner or Vendor Centers.

You can customize the URL of your linked form so that certain information can automatically be sent to NetSuite after the form is submitted. These are called parameters, and the information sent to the relevant field in NetSuite can't be modified by customers.

For example, Wolfe Electronics wants to include a link to the case form from one of their microsites. After setting up the new case origin type, they include the parameter &origin=Cameras to track the case origin from their camera business. (Case origin types are located at _Setup > Support > Case Origin Types_.) Now, when someone submits the form, 'Cameras' is automatically entered in the Case Origin field on the form. This field can be set to hidden if required.

To add this parameter to the publishable form URL, add the &origin=Cameras parameter to the end of the URL. NetSuite adds several parameters to the URL by default, don't overwrite these when adding additional parameters.

Below is a list of supported parameters and example text for each one.

| **Field** | **Tag and Example** |
| --- | --- |
| Company Name | &companyname=Global Distributing |
| Email | &email=john@example.com |
| Message | &incomingmessage=This is the message. |
| Subject/Title | &title=Problem With Service |
| Subsidiary | &subsidiary=UK |
| Case Origin | &origin=Online |
| Case Type | &category=Service Problem |
| Phone Number | &phone=555-555-5555 |
| Contact First Name | &firstname=John |
| Contact Last Name | &lastname=Doe |
| Contact Middle Name | &middlename=Lee |
| Start Date | &startdate=11/11/2005 |
| Start Time | &starttime=12:00 pm |
| Support Issue | &issue=Issue |
| Support Item | &item=Item |

### Related Topics

-   [Creating an Online Case Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162307025197.html)
-   [Uploading Files Through an Online Case Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2429734.html)
-   [Custom HTML Form Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2429943.html)
-   [Online Case Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2428291.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
