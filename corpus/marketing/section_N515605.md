---
id: "section_N515605"
type: "section"
title: "Using CRMSDK Tags"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Email Marketing Campaigns > Working with Email Templates > Using CRMSDK Tags"
parent: "section_N514744"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N515605.html"
anchors: ["bridgehead_N520067", "bridgehead_N520220", "bridgehead_N520812", "bridgehead_N521522", "bridgehead_N523278"]
sha256: "84b350d53fcc9be65b29dcda006cef8d6543776f1fdfa9b579a172ab955ae36f"
---

You use CRMSDK tags to customize PDF and letter templates. When a template generates a document, NetSuite replaces the CRMSDK tags with the information in the corresponding fields on the recipient's record.

The following table includes the CRMSDK tags recognized by NetSuite.

The entries in the Field column refer to fields on CRM records you can reference in your templates. An " **x** " marks the records that include each field.

| **Field** | **Cust:Project** | **Vendor** | **Partner** | **Employee** | **Contact** | **Tag** |
| --- | --- | --- | --- | --- | --- | --- |
| Auto Name | x | x | x | x | x | NLAUTONAME |
| Company Name | x | x | x | x |  | NLCOMPANYNAME |
| Name | x | x | x | x | x | NLENTITYID |
| Sales Rep | x |  |  |  | **†** | NLSALESREP |
| Phone | x | x | x | x | x | NLPHONE |
| Alt. Phone | x | x |  |  |  | NLALTPHONE |
| Fax | x | x | x |  | x | NLFAX |
| Email | x | x | x | x | x | NLEMAIL |
| Contact First Name | x | x |  |  | x | NLFIRSTNAME |
| Contact Last Name | x | x |  |  | x | NLLASTNAME |
| Contact Middle Initial |  |  |  | x | x | NLMIDDLENAME |
| Promotion Code | x |  |  |  | **†** | NLREFERRALCODE |
| Partner | x |  |  |  | **†** | NLPARTNER |
| Child Of, Subpartner Of, Company | x |  | x |  | x | NLCOMPANY |
| Child Of | x |  |  |  |  | NLPARENT |
| Address Line 1 | x | x | x | x | x | NLADDRESS1 |
| Address Line 2 | x | x | x | x | x | NLADDRESS2 |
| City | x | x | x | x | x | NLCITY |
| State/County | x | x | x | x | x | NLSTATE |
| Zip/Postal Code | x | x | x | x | x | NLZIPCODE |
| Country | x | x | x | x | x | NLCOUNTRY |
| Account Number | x | x |  | x | **†** | NLACCOUNTNUMBER |
| Terms | x | x |  |  | **†** | NLTERMS |
| Balance | x |  |  |  |  | NLBALANCE |
| Days Overdue | x |  |  |  |  | NLDAYSOVERDUE |
| Overdue Balance | x |  |  |  |  | NLOVERDUEBALANCE |
| Sales Rep Nickname | x |  |  |  |  | NLSALESREPNICKNAME |
| Signature | x |  |  |  |  | NLSIGNATURE |
| Salutation |  |  |  | x | x | NLSALUTATION |
| Department |  |  |  | x |  | NLDEPARTMENT |
| Class |  |  |  | x |  | NLCLASS |
| Location |  |  |  | x |  | NLLOCATION |
| Supervisor |  |  |  | x | x | NLSUPERVISOR |
| Alt. Email |  |  |  |  | x | NLALTEMAIL |
| Office Phone |  |  |  |  | x | NLOFFICEPHONE |
| Home Phone |  |  |  |  | x | NLHOMEPHONE |
| Mobile Phone |  |  |  |  | x | NLMOBILEPHONE |
| Title/Subject |  |  |  |  | x | NLTITLE |
| Partner Code |  |  | x |  |  | NLPARTNERCODE |

Note:

The preceding table lists the most commonly used CRMSDK tags and the corresponding fields. To see a complete list of supported tags, open a letter template file in NetSuite. Go to Documents > Templates > Letter Templates > New. From the Templates subtab, click the Download link to open an Excel file containing all tags.

CRMSDK tags have different formats depending on where they are used. CRMSDK tags should always be capitalized. Use the following formats:

-   **PDF templates** - enter without brackets
    
-   **Letter templates** - automatically formatted by Microsoft Word
    

In general, the tags you apply to a template must match the record for the document you create. For example, you can't use a template to create a partner letter if the template includes a tag for the Sales Rep field.

However, if you create a template to communicate with contacts, you can refer to fields on the parent record associated with the contact. For example, you can include the name of the sales rep assigned to a customer in a message sent to that customer's contact person.

In addition, you can use fields in contact templates that do not appear on the contact record. In the preceding table, these fields appear with a " **†** ".

When you include the NLFIRSTNAME and NLLASTNAME tags in a template, NetSuite replaces these tags based on these rules:

-   If the recipient is a customer of the type Individual, NetSuite uses the first and last name on the customer record.
    
-   If the recipient is a customer of the type Company, NetSuite uses the primary contact's first and last name.
    

## Inserting Tags for Names {#bridgehead_N520067}

When you create an email template for customers, you can use the following tags:

-   **NLENTITYID** - This tag inserts the information entered in the Customer ID field.
    
    To add this field to a template, select Name in the Insert Field.
    
-   **NLCOMPANYNAME** - This is the information entered in the Company Name field on the customer record.
    
    To add this field to a template, select Company Name in the Insert Field.
    
-   **NLFIRSTNAME** - This is the information entered in the first name field. This applies only to customers who are individuals.
    
    To add this field to a template, select First Name in the Insert Field.
    
-   **NLLASTNAME** - This is the information entered in the last name field. This applies only to customers who are individuals
    
    To add this field to a template, select Last Name in the Insert Field.
    
-   **NLCONTACT** - This is the name of the customer's primary contact.
    
    Select Contact (Primary) in the Insert Field
    

When you create a template for contacts, you can use the following:

-   **NLENTITYID** - This tag inserts the information entered in the Contact ID field.
    
    To add this field to a template, select Name in the Insert Field.
    
-   **NLCOMPANY** - This is the information in the Customer ID field on the customer record for which this contact is the primary.
    
    To add this field, select Parent Entity in the Insert Field.
    
-   **NLFIRSTNAME** - This is the information entered in the first name field on the contact record.
    
    To add this field to a template, select First Name in the Insert Field.
    
-   **NLLASTNAME** - This is the information entered in the last name field on the contact record.
    
    To add this field to a template, select Last Name in the Insert Field.
    

## CRMSDK Tags for Cases {#bridgehead_N520220}

You can use the following tags to add case information to a document. You can use these tags in addition to the CRMSDK tags that refer to the customer who entered the case.

| Field | Tag |
| --- | --- |
| Subject | NLTITLE |
| Case Number | NLCASENUMBER |
| Company Name | NLCOMPANYNAME |
| Support Rep Assigned | NLASSIGNED |
| Priority | NLPRIORITY |
| Contact Name | NLCONTACT |
| Status | NLSTATUS |
| Origin | NLORIGIN |
| Message History (Non-Internal) | NLCASEHISTORY |
| Message History (Internal or External) | NLCASEHISTORYEMP |
| Most Recent (Non-Internal) Message | NLCASELASTMESSAGE |
| Most Recent Message (Internal or External) | NLCASELASTMESSAGEEMP |
| Creation Time | NLSTARTTIME |
| Creation Date | NLSTARTDATE |
| Type | NLCATEGORY |
| Recent Escalation Message | NLESCALATIONMESSAGE |
| Link to Customer Center | NLCASEURL |
| Name of User who Logged In | NLUSERNAME |
| Company Logo | NLCOMPANYLOGO |
| Signature | NLSIGNATURE |

Note:

The following tags are not supported for use in PDF or letter templates:

-   NLCASEHISTORY
    
-   NLCASEHISTORYEMP
    
-   NLCASELASTMESSAGE
    
-   NLCASELASTMESSAGEEMP
    

## CRMSDK Tags for Issues {#bridgehead_N520812}

You can use the following tags to add issue information to documents. You can use these tags in addition to the CRMSDK tags that refer to cases associated with an issue.

| Field | Tag |
| --- | --- |
| Abstract | NLISSUEABSTRACT |
| Assigned To | NLASSIGNEDTO |
| Broken In Build | NLBUILDBROKEN |
| Broken In Version | NLVERSIONBROKEN |
| Creation Date | NLISSUECREATEDDATE |
| Creation Time | NLISSUECREATEDTIME |
| Duplicate Number | NLISSUEDUPLICATEOF |
| External Abstract | NLEXTERNALABSTRACT |
| External Details | NLEXTERNALDETAILS |
| External Status | NLEXTERNALSTATUS |
| External Target | NLEXTERNALTARGET |
| Fixed In Build | NLBUILDFIXED |
| Fixed In Version | NLVERSIONFIXED |
| Number | NLISSUENUMBER |
| Priority | NLISSUEPRIORITY |
| Product | NLPRODUCT |
| Product Team | NLPRODUCTTEAM |
| Reviewer | NLREVIEWER |
| Severity | NLSEVERITY |
| Showstopper | NLISSHOWSTOPPER |
| Status | NLISSUESTATUS |
| Target Build | NLBUILDTARGET |
| Target Version | NLVERSIONTARGET |
| Type | NLISSUETYPE |

## CRMSDK Tags for Transactions {#bridgehead_N521522}

You can use the following tags to include transaction information in messages you send.

| Field | Tag |
| --- | --- |
| Bill To | NLBILLADDRESS |
| Class | NLCLASS |
| Consolidated Balance | NLCONSOLBALANCE |
| (Consolidated) Overdue | NLCONSOLOVERDUEBALANCE |
| (Consolidated) Days | NLCONSOLDAYSOVERDUE |
| Currency | NLCURRENCYNAME |
| Date | NLTRANDATE |
| Date Created | NLDATECREATED |
| Days Open | NLDAYSOPEN |
| Department | NLDEPARTMENT |
| Exchange Rate | NLEXCHANGERATE |
| Expected Close Date | NLEXPECTEDCLOSEDATE |
| Forecast Type | NLFORECASTTYPE |
| ID | NLID |
| Include in Forecast | NLINCLUDEINFORECAST |
| Include in Forecast: High | NLINCLUDEINFORECASTHIGH |
| Include in Forecast: Low | NLINCLUDEINFORECASTLOW |
| Project | NLJOB |
| Last Modified Date | NLLASTMODIFIEDDATE |
| Lead Source | NLLEADSOURCE |
| Location | NLLOCATION |
| Main Entity | NLENTITY |
| Memo | NLMEMO |
| Open Status | NLOPENSTATUS |
| Partner | NLPARTNER |
| Probability | NLPROBABILITY |
| Sales Group | NLSALESGROUP |
| Sales Rep/Employee | NLSALESREP |
| Ship To | NLSHIPADDRESS |
| Status | NLDOCUMENTSTATUS |
| Total | NLTOTAL |
| Transaction # | NLTRANID |
| Type | NLTYPE |

## Custom Field Tags {#bridgehead_N523278}

To determine the tags to use for custom fields, enable the Show Internal IDs preference at Home > Set Preferences > General. Then, click the field name to open the field-level help popup. NetSuite displays the field ID in the bottom right corner of the popup. You create a CRMSDK tag when you prepend this ID with **NL**.

A custom field CRMSDK tag might look like this:

**NLCUSTENTITY5**

Note:

If you include tags for rich text custom fields in templates, NetSuite does not preserve font formats in tag replacements in the final message. Font formatting includes color, bold, size, and so on.

### Related Topics

-   [Sending Email from NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N512264.html)
-   [Working with Email Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N514744.html)
-   [Email Marketing Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1001310.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
