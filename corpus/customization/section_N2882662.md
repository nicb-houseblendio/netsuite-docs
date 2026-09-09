---
id: "section_N2882662"
type: "section"
title: "Creating Online Custom Record Forms"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Records Overview > Creating Custom Record Types > Online Custom Record Forms > Creating Online Custom Record Forms"
parent: "section_N2882522"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2882662.html"
anchors: ["procedure_N2882675"]
sha256: "1e9a99722927c40776f60f9cfe24b99e705ee60e5a97a98803b33ab096fcb4c4"
---

You can create an online custom record form to receive information from customers on your website.

#### To create an online custom record form: {#procedure_N2882675}

1.  Go to _Customization > Lists, Records, & Fields > Record Types_.
    
2.  In the **Edit** column, click the name of the record you want to create an online form for.
    
3.  In the **Online Forms** subtab, click **New Online Form** or **New Online HTML Form**.
    
    Selecting **New Online Form** enables you to create a form based on the NetSuite default template. Selecting **New Online HTML Form** lets you create a form based on a custom HTML template you've created. You must first create the custom HTML template before you can use it for an online form.
    
    The steps involved for creating an Online Form versus an Online HTML Form are the same with a couple of exceptions as noted in the following procedure.
    
4.  Enter a title for this form.
    
    This title is displayed at the top of the form.
    
5.  If creating an HTML template (these options **aren't** available for Default templates):
    
    -   In the **Template** field, select the HTML template you want to use for this form.
        
        You can create online HTML form templates at Lists > Marketing > Marketing Templates.
        
    -   To have NetSuite insert labels for your form fields, check the **Include Field Labels** box.
        
        If you leave this box unchecked, you must include field labels in your HTML template file.
        
6.  If creating a Default template (these options **not** available for HTML templates):
    
    -   In the **Message** field, enter a message to display at the top of the form.
        
        This message can include up to 500 HTML characters.
        
        Note:
        
        The message can be formatted using built-in rich text formatting tools. If you prefer to edit the message directly with HTML tags, click **Source**.
        
    -   In the **Detail Message** field on the **Detail Message** subtab, enter a message to display at the bottom of the form.
        
        This message can include up to 4000 HTML characters. Again, you can use the built-in rich text formatting tools or view as HTML only.
        
7.  If you want to link to this form from a website, check the **Enable Online** box.
    
8.  If required, check the **Inactive** box. You can always reactivate it at a later date.
    
9.  In the **Select Fields** subtab, edit any existing fields or add new fields as needed.
    
10.  Rearrange the order of fields as needed. Click a line and drag it to the required position or click **Move Up**, **Move Down**, **Move to Top** or **Move to Bottom**.
     
11.  In the **Set Up Workflow** subtab:
     
     -   To receive notification when this form is submitted, enter the addresses you want email messages to be sent to in the **Notify by Email** field.
         
     -   To specify a page for customers to be sent to after they submit the form, enter the URL for that page in the **Redirect to URL** field. By default, the user who submits the form is redirected the home page of your primary website.
         
     -   In the **Handle Duplicate Records** field, select how you want NetSuite to handle records that are duplicates of existing records.
         
12.  In the **Set Up Appearance** subtab:
     
     With the exception of the Font, the fields described in the following list apply only to default templates.
     
     -   In the **Number of Columns Shown** field, select the number of columns for the form.
         
     -   In the **Color Theme** field, select a color theme for the form.
         
     -   In the **Font** field, select a font for the form.
         
     -   To expand any subtabs on the form, check the **Unlayered Sections** box.
         
     -   In the **Button Alignment** field, select where to place the buttons on the form.
         
     -   In the **Form Logo** field, select a logo to place at the top of the form.
         
         You can upload new logos at _Setup > Intranet > Images_ or _Commerce > Site Builder > Content > Images_.
         
         As you define the appearance options for your form, keep in mind that your end users use various sized browsers and types. For example, if you're designing on a high-resolution large monitor, several columns may display fine. However, for smaller low-resolution monitors it can be better to construct your layout with fewer columns. Also, if customers may need to print the form, ensure that the colors you select will properly display for both color and black and white printers.
         
13.  In the **Custom Code** subtab:
     
     The **Custom Code** subtab is available only if you have a SuiteScript feature enabled. For detailed information about using custom JavaScript files to perform functions, refer to [SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/set_1502135122.html).
     
     -   In the **Script File** field, select the JavaScript file that contains the required scripts for this form.
         
         Important:
         
         You must upload your file to the File Cabinet before you can select it. Client script file records or files referenced in client scripts must not have the **Hide in SuiteBundle** preference enabled.
         
     -   In the **Page Init Function** field, enter the script name to be called from your script file when this entry form is first loaded.
         
     -   In the **Save Record Function** field, enter the script name to be called from your script file when this record is saved.
         
     -   In the **Validate Field Function** field, enter the script name to be called from your script file when a field on this entry form is changed.
         
     -   In the **Field Changed Function** field, enter the script name to be called from your script file when a change made to a field is accepted.
         
14.  Click **Save**.
     
15.  If needed, preview your new form.
     
     Select the form from the Online Form subtab and then click **Preview**.
     
16.  Add links to your online form to your website.
     
     For details on how link to your online form see [Creating Links to Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880942.html).
     

Now, customers can enter information about your website, and records are automatically created or updated in NetSuite.

### Related Topics

-   [Online Custom Record Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2882522.html)
-   [Adding Custom Online Forms for a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2879167.html)
-   [Linking Online Custom Record Forms to My Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2883101.html)
-   [Creating HTML Templates for Online Custom Record Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2885246.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
