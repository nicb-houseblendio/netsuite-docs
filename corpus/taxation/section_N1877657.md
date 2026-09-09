---
id: "section_N1877657"
type: "section"
title: "Setting Up Tax Filing for Czechia"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Czechia Tax Topics > Setting Up Tax Filing for Czechia"
parent: "chapter_N1874317"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1877657.html"
anchors: ["bridgehead_N1877711", "procedure_N1877720", "bridgehead_N1878776", "procedure_N1878786"]
sha256: "52493307d7bdc6e3ea450b90a9a3e7e61b7dfb57a44b3aa9557c66bd7de2b234"
---

If you have a Czechia nexus and you intend to use the NetSuite to generate your Czechia VAT return and EU sales list, you must set up your online tax filing details before you generate the report. This feature requires the [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html) SuiteApp. For more information, read the following topics:

-   [VAT Online Filing Setup](#bridgehead_N1877711)
    
-   [EU Sales List Online Filing Setup](#bridgehead_N1878776)
    

## VAT Online Filing Setup {#bridgehead_N1877711}

With the International Tax Reports SuiteApp, you can set up VAT online filing for Czechia

#### To set up VAT online filing for Czechia: {#procedure_N1877720}

1.  Go to Reports > VAT/GST > Tax Reports (International).
    
2.  Select your Czechia VAT-registered subsidiary.
    
3.  Click **Setup**, and select **Tax Filing**.
    
4.  Choose or enter values in the fields of the Online Filing Setup page.
    
    Note:
    
    The fields on this page are used to complete Sections A and B of the XML file of the VAT return. The Czechia VAT form displayed in NetSuite contains only Section C, which shows transaction amounts and VAT amounts. The XML file NetSuite generates meets tax agency requirements and can be used for online tax filing. You can submit the XML file to your tax agency's Web portal.
    
    Important:
    
    You must fill in all required fields (marked with \*) before you can generate the XML file for the VAT report
    
    | Field | Description |
    | --- | --- |
    | **SECTION A** |
    | Tax Returns | Choose the type of tax return to be filed: **B** - the tax return is correct **O** - the tax return is being filed to correct a previous return **D** - the tax return contains additions **E** - the tax return contains additions and corrections |
    | Code of tax period the following year | Choose the tax period code: **Q2** - if turnover for the previous calendar year reached 2,000,000 and tax period is a quarter **M10** - if turnover for the previous year amounted to CZK 10 million and tax period is a month **Q** - if turnover for the previous calendar year reached the amount of CZK 10 million, and tax period is a quarter **M** - if turnover for the previous year amounted to at least 2 million CZK, but has not reached the amount of CZK 10 million, and tax period is a month |
    | Payer Type | Choose the payer type:
    -   **Taxpayer**
    -   **Group**
    -   **Person identified for tax**
    
     |
    | If no data exists for page 2, cross out (X) | If the tax return has no data on page 2 (SECTION C), check this box to place a cross mark (X) on this field on the VAT return |
    | Type of Taxpayer | Choose the type of taxpayer:
    
    -   **F** - individual
    -   **P** - a legal entity
    
     |
    | \*Revenue Office | Enter the 3-digit code of the tax office. |
    | \*Tax Identification No. | Enter the 10-digit tax identification number of the taxpayer. |
    | Company Name | Enter the company name. |
    | City | Enter the name of the company's city. |
    | Post code | Enter the company's post code. |
    | Telephone | Enter the company's phone number. |
    | Street | Enter the company's street address. |
    | E-mail | Enter the company's email address. |
    | Country | Enter the company's country. |
    | Main economic activity | Enter the company's main economic activity. |
    | **SECTION B** |
    | Type of representative | In case of a group, choose the type of representative (group member) who is filing this tax return:
    
    -   **F** - individual
    -   **P** - a legal entity
    
     |
    | Code of the representative | Choose the code of the representative:
    
    -   **1** - guardian
    -   **2** - appointed representative
    -   **3** - joint representative agent
    -   **4a** - attorney general (person or legal entity)
    -   **4b** - individual tax advisor or lawyer (person)
    
     |
    | Last name | Enter the representative's last name. |
    | Name | Enter the representative's first name. |
    | Date of birth | Enter the representative's date of birth. |
    | Registration number of the tax consultant | If a tax consultant is filing this tax return, enter their registration number. |
    | Name of the legal entity | If a legal entity is filing this tax return, enter the name of the legal entity. |
    | ID of the legal entity | If a legal entity is filing this tax return, enter the ID of the legal entity. |
    | **INDIVIDUAL AUTHORIZED TO SIGN** |
    | Last name | Enter the last name of the person authorized to sign this tax return. |
    | Name | Enter the first name of the person authorized to sign this tax return. |
    | Relationship to the legal entity | Enter the relationship of this authorized person to the legal entity. |
    | **The declaration was compiled by** |
    | Last name | Enter the last name of the person who compiled this tax declaration. |
    | Name | Enter the first name of the person who compiled this tax declaration. |
    | Telephone | Enter the phone number of the person who compiled this tax declaration. |
    | VAT Reporting Period | Select the VAT reporting period for your VAT return submissions.
    
    -   **By Month**
    -   **By Quarter**
    
     |
    
5.  Click **Save**.
    

## EU Sales List Online Filing Setup {#bridgehead_N1878776}

#### To set up EU sales list online filing for Czechia: {#procedure_N1878786}

1.  Go to Reports > VAT/GST > EU Sales List Report.
    
2.  Select your Czechia VAT-registered subsidiary.
    
3.  Click **Setup**, and select **EU Sales Filing**.
    
4.  Choose or enter values in the fields of the EU Sales Filing Setup page.
    
    Important:
    
    You must fill in all required fields (marked with \*) before you can generate the XML file for the VAT report
    
    | Field | Description |
    | --- | --- |
    | Form SH | Choose the type of report to be filed:
    -   **R** - Recapitulative Statement
    -   **N** - Corrective Recapitulative Statement
    
     |
    | Type of Taxpayer | Choose the type of taxpayer:
    
    -   **F** - individual
    -   **P** - a legal entity
    
     |
    | \*Revenue Office | Enter the 3-digit code of the tax office. |
    | \*Tax Identification No. | Enter the 10-digit tax identification number of the taxpayer. |
    | Company Name | Enter the name of the company. |
    | City | Enter the name of the company's city. |
    | Post code | Enter the company's post code. |
    | Telephone | Enter the company's phone number. |
    | Street | Enter the company's street address. |
    | Type of representative | In case of a group, choose the type of representative (group member) who is filing this tax return:
    
    -   **F** - individual
    
    -   **P** - a legal entity
    
     |
    | Code of the representative | Choose the code of the representative:
    
    -   **1** - guardian
    -   **2** - appointed representative
    -   **3** - joint representative agent
    -   **4a** - attorney general (person or legal entity)
    -   **4b** - individual tax advisor or lawyer (person)
    
     |
    | Last name | Enter the representative's last name. |
    | Name | Enter the representative's first name. |
    | Date of birth | Enter the representative's date of birth. |
    | Registration number of the tax consultant | If a tax consultant is filing this tax return, enter the consultant's registration number. |
    | Name of the legal entity | If a legal entity is filing this tax return, enter the name of the legal entity. |
    | ID of the legal entity | If a legal entity is filing this tax return, enter the ID of the legal entity. |
    | **INDIVIDUAL AUTHORIZED TO SIGN** |
    | Last name | Enter the last name of the person authorized to sign this tax return. |
    | Name | Enter the first name of the person authorized to sign this tax return. |
    | Relationship to the legal entity | Enter the relationship of this authorized person to the legal entity. |
    | **The declaration was compiled by** |
    | Last name | Enter the last name of the person who compiled this tax declaration. |
    | Name | Enter the first name of the person who compiled this tax declaration. |
    | Telephone | Enter the phone number of the person who compiled this tax declaration. |
    | VAT Reporting Period | Select the VAT reporting period for your EU sales list submissions.
    
    -   **By Month**
    -   **By Quarter**
    
     |
    
5.  Click **Save**.
    

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Czechia Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1874517.html)
-   [Czechia VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1880287.html)
-   [Czechia VAT Control Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4491314862.html)
-   [EU Sales List for Czechia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1884938.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
