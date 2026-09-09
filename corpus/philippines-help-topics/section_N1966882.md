---
id: "section_N1966882"
type: "section"
title: "Withholding Tax Reports - Philippines"
branch: "philippines-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Philippines Help Topics > Philippines Tax Topics > Withholding Tax Reports - Philippines"
parent: "chapter_N1950898"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1966882.html"
anchors: ["bridgehead_N1966961", "procedure_N1966976", "bridgehead_N1967045", "procedure_N1967062", "bridgehead_1539935368", "bridgehead_0114014022", "bridgehead_0224094312", "procedure_47094523678", "bridgehead_N1967125", "procedure_N1967141", "bridgehead_0121100446", "procedure_13100628111", "bridgehead_0224095554", "procedure_42095834276", "procedure_55100711392", "bridgehead_N1967231", "procedure_N1967248"]
sha256: "59c88ae8d90e94257758bed763f457cfcf614b6a3a223b3ab61c8c70b0659997"
---

The Withholding Tax SuiteApp provides the following withholding tax reports for the Philippines:

-   [Certificate of Creditable Tax Withheld at Source (Form 2307)](#bridgehead_N1966961)
    
-   [Monthly Remittance Return of Creditable Income Taxes Withheld (Expanded) (Form 1601-E)](#bridgehead_N1967045)
    
-   [Quarterly Remittance Return of Creditable Income Taxes Withheld (Expanded) (Form 1601-EQ)](#bridgehead_1539935368)
    
-   [Monthly Remittance Form of Creditable Income Taxes Withheld (Expanded) (Form 0619-E)](#bridgehead_0114014022)
    
-   [Monthly Remittance Form of Final Income Taxes Withheld (Form 0619-F)](#bridgehead_0224094312)
    
-   [Quarterly Alphalist of Payees (QAP)](#bridgehead_N1967125)
    
-   [Annual Alphalist of Payees (1604E)](#bridgehead_0121100446)
    
-   [Payment Form (0605)](#bridgehead_0224095554)
    
-   [Summary Alphalist of Withholding Tax Agents/Payors of Income Payments subjected to Creditable Withholding Tax at Source (SAWT)](#bridgehead_N1967231)
    

**Online Filing of Withholding Tax Reports**

The Philippines tax agency, Bureau of Internal Revenue, issued Revenue Regulations No. 1-2014 which requires the electronic submission of the alphabetical list of payees of income payments as attachment to tax returns filed online.

With the Withholding Tax SuiteApp, you can generate the Quarterly Alphalist of Payees (QAP), Annual Alphalist of Payees, and Summary Alphalist of Withholding Taxes (SAWT) reports in DAT format as prescribed by the BIR.

Note:

When available, the Withholding Tax SuiteApp uses the information saved on the Tax Filing Setup page (from International Tax Reports) in the QAP and SAWT report DAT files. Make sure the information you entered on the Tax Filing Setup page complies with the requirements of the BIR Alphalist Data Entry and Validation Module. For more information, see [Setting Up Tax Filing for the Philippines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1955261.html).

When you generate the QAP or SAWT report, click the **Export - DAT** button to export a DAT file of the report. The generated DAT file can be attached to tax returns for online tax filing.

## Certificate of Creditable Tax Withheld at Source (Form 2307) {#bridgehead_N1966961}

The Certificate of Creditable Tax Withheld at Source (Form 2307) is a certificate issued by payors of income to the payee, showing the amount paid and the amount of tax withheld from income payments that are subject to creditable tax. This certificate is submitted by the payee to the Bureau of Internal Revenue to claim a tax credit or refund.

The Form 2307 is part of the implementation of the Philippines Tax Reform for Acceleration and Inclusion (TRAIN) Law.

#### To generate Form 2307: {#procedure_N1966976}

1.  Go to Reports > Withholding Tax > Withholding Tax Reports.
    
2.  In the **Subsidiary** field, select a Philippines subsidiary.
    
3.  In the **Reports** field, select **Form 2307**.
    
4.  Select the tax period for the report.
    
5.  Select the tax type used for creditable withholding tax.
    
6.  Select a **Vendor** (Payee).
    
7.  Click the **Refresh** button to load the report based on your selected criteria.
    
    Important:
    
    Click **Refresh** each time you change the reporting criteria (tax period, tax type, or vendor).
    
8.  If you want to generate a report that includes only selected transactions from the vendor, click the **Select Transactions** button.
    
    -   Transactions with a checked box are included in the report. To exclude a transaction, clear the box next to it. To exclude all transactions on the current page, clear the box in the column header.
        
    -   To select a page to view, use the paging toolbar at the bottom of the page. Click the arrows to go to the next page, or type the page number and press **Enter**.
        
    -   Click **Save** to save your selected transactions.
        
    
    Upon saving, the report will reload to show only your selected transactions.
    
9.  Fill out the information as required in the manual input fields, such as:
    
    -   Taxpayer Identification Number
        
    -   Payee's Name
        
    -   Registered Address
        
    -   Zip Code
        
    -   Foreign Address (if applicable)
        
    
    Under **Signatory Details:**
    
    -   Payor/Authorized Representative/Tax Agent
        
    -   Tax Agent Accreditation No./Attorney's Roll No.
        
    -   Payee/Authorized Representative/Tax Agent
        
    -   Tax Agent Accreditation No./Attorney's Roll No.
        
10.  To download a PDF file of the Form 2307 containing all selected transactions, click **Print**.
     
11.  To download individual forms for each transaction in the report, click **Print Individual 2307**. A compilation of the individual Form 2307 for each transaction will be generated in a single PDF file.
     
     Note:
     
     If you want to print individual Form 2307 for each transaction, you should set the tax period to one month to avoid performance issues.
     

## Monthly Remittance Return of Creditable Income Taxes Withheld (Expanded) (Form 1601-E) {#bridgehead_N1967045}

The Monthly Remittance Return of Creditable Income Taxes Withheld (Expanded) or Form 1601-E is the form used for the monthly filing and payment of creditable (expanded) withholding tax, prior to the implementation of TRAIN Law (RA No. 10963)

#### To generate Form 1601-E: {#procedure_N1967062}

1.  Go to Reports > Withholding Tax > Withholding Tax Reports.
    
2.  Select a Philippines subsidiary in the **Subsidiary** field or select **Philippines** in the **Nexus** field.
    
3.  In the **Reports** field, select **Form 1601-E**.
    
4.  Select the tax period for the report.
    
5.  Select the tax type used for creditable withholding tax.
    
6.  Click **Print** to download a PDF file of the report.
    
    Important:
    
    Click **Refresh** each time you change the reporting criteria (tax period or tax type).
    

## Quarterly Remittance Return of Creditable Income Taxes Withheld (Expanded) (Form 1601-EQ) {#bridgehead_1539935368}

Under the TRAIN Law (RA No. 10963), the creditable (expanded) withholding tax return is due quarterly, and remitted through the Quarterly Remittance Return of Creditable Income Taxes Withheld (Expanded) (Form 1601-EQ). Remittance is done on or before the last day of the month following the close of the calendar quarter.

#### To generate Form 1601-EQ:

1.  Go to Reports > Withholding Tax > Withholding Tax Reports.
    
2.  Select a Philippines subsidiary in the **Subsidiary** field or select **Philippines** in the **Nexus** field.
    
3.  In the **Reports** field, select **Form 1601-EQ**.
    
4.  Select the tax period for the report.
    
5.  Select the tax type used for creditable withholding tax.
    
6.  Click **Print** to download a PDF file of the report.
    

Important:

Click **Refresh** each time you change the reporting criteria (tax period or tax type).

## Monthly Remittance Form of Creditable Income Taxes Withheld (Expanded) (Form 0619-E) {#bridgehead_0114014022}

The Monthly Remittance Form if Creditable Income Taxes Withheld (Expanded) or Form 0619-E is used for reporting and remitting income taxes that have been deducted or withheld from various income payments.

#### To generate Form 0619-E:

1.  Go to Reports > Withholding Tax > Withholding Tax Reports.
    
2.  Select a Philippines subsidiary in the **Subsidiary** field or select **Philippines** in the **Nexus** field.
    
3.  In the **Reports** field, select **Form 0619-E**.
    
4.  In the **Tax Period** field, select the tax period for the report.
    
5.  Select **Tax Type** field, select the tax type used for creditable income tax.
    
6.  The **Part II - Tax Remittance** section of the form shows boxes 14 - 18:
    
    1.  **14 Amount of Remittance** - This box shows the total calculated withholding tax for the selected tax period and tax type. The value on this box is sourced from various transactions with calculated withholding tax amounts.
        
    2.  **15****Less: Amount Remitted from Previously Filled Form, if this is an amended form** - Enter the applicable value to deduct from the amount of remittance.
        
    3.  **16 Net Amount of Remittance (Item 14 Less Item 15)** - This box shows the calculated net amount of remittance by deducting the value of box 15 from box 14.
        
    4.  **17 Add: Penalties:** - Enter the applicable values for boxes 17A - 17C. Box 17D shows the total amount of penalties.
        
    5.  **18 Total Amount of Remittance** - This box shows the total amount of calculated remittance by adding the values from box 16 and 17D.
        
7.  Click **Print** to download a PDF file of the report.
    

Important:

Click **Refresh** each time you change the reporting criteria (tax period or tax type).

## Monthly Remittance Form of Final Income Taxes Withheld (Form 0619-F) {#bridgehead_0224094312}

Use the Monthly Remittance Form of Final Income Taxes Withheld or Form 0619-F for reporting and remitting income taxes that have been deducted or withheld from various income payments subject to Final Withholding Taxes.

#### To generate Form 0619-F reports: {#procedure_47094523678}

1.  Go to Reports > Withholding Tax > Withholding Tax Reports.
    
2.  Select a Philippines subsidiary in the **Subsidiary** field or select **Philippines** in the **Nexus** field.
    
3.  Select **Form 0619-F** in the **Reports** field.
    
4.  Select the relevant tax period in the **Tax Period** field.
    
5.  Select the tax type used for final income taxes in the **Tax Type** field.
    
6.  Select the relevant alphanumeric tax code in the **ATC** field.
    
    -   **WMF10** - If selected, **WB** is set as the Tax Type Code value in printed 0619-F reports.
        
    -   **WMF20** - If selected, **WF** is set as the Tax Type Code value in printed 0619-F reports.
        
7.  Provide or review values in the following manual input fields:
    
    -   **13** - If you selected WMF10 from the ATC list, this box shows the amount of final income taxes withheld. If you selected WMF20 instead, the listed value is 0.00.
        
    -   **14** - If you selected WMF20 from the ATC list, this box shows the amount of final income taxes withheld. If you selected WMF10 instead, the listed value is 0.00.
        
    -   **15** - This box shows the calculated total amount of final income taxes withheld.
        
    -   **16** - Enter the applicable value to deduct from the remittance amount.
        
    -   **17** - This box shows the net amount of remittance calculated by deducting the value of box 15 from that of box 16.
        
    -   **18A** - Enter the applicable additional charge or payment penalty.
        
    -   **18B** - Enter the applicable amount of interest penalty.
        
    -   **18C** - Enter the applicable amount of compromise penalty.
        
    -   **18D** - This box shows the total penalties calculated by adding the values of boxes 18A - 18C.
        
    -   **19** - This box shows the total amount of remittance calculated by adding the values of boxes 17 and 18D.
        
8.  Click **Print** to download a PDF file of the report.
    
    The following footer information appears on the bottom right of every printed Form 0619-F:
    
    -   First line: Printed by `<user + user ID>` on `<date and time stamp>`
        
    -   Second line: Oracle NetSuite (edition) (version)
        

## Quarterly Alphalist of Payees (QAP) {#bridgehead_N1967125}

The Quarterly Alphalist of Payees (QAP) is a consolidated alphabetical listing of income earners from whom a part of income was withheld as tax and remitted by the income payors to the Bureau of Internal Revenue.

This list is submitted by the income payor as an attachment to tax returns filed for a specified period. The list shows, among others, the registered name of the income payees, and their tax identification numbers (TIN), as well as the nature and amounts of income paid.

#### To generate a QAP: {#procedure_N1967141}

1.  Go to Reports > Withholding Tax > Withholding Tax Reports.
    
2.  In the **Subsidiary** field, select a Philippines subsidiary.
    
3.  In the **Reports** field, select **Quarterly Alphalist of Payees (QAP)**.
    
4.  Select the tax period for the report.
    
5.  Select a tax type to generate a report for. Only tax types of the nexus associated with the subsidiary are available for selection.
    
6.  Click **Submit**.
    
7.  When the report is displayed, click any of the following options:
    
    -   **Print PDF**
        
    -   **Export - CSV**
        
    -   **Export - DAT**
        
    -   **Return to Criteria**
        

## Annual Alphalist of Payees (1604E) {#bridgehead_0121100446}

Use the Annual Alphalist of Payees (1604E) for reporting of income earners for an annual period. This report includes an alphabetical listing of earners from whom a part of income was withheld as tax and remitted by the income payors to the Bureau of Internal Revenue. 1604E - schedule 3 is an attachment to BIR Form 2307, which NetSuite supports.

This list is submitted by the income payor as an attachment to tax returns filed for a specified period. The list shows, among others, the registered names of the income payees, and their tax identification numbers (TIN), as well as the nature and amounts of income paid.

#### To generate a 1604E: {#procedure_13100628111}

1.  Go to Reports > Withholding Tax > Withholding Tax Reports.
    
2.  In the **Subsidiary** field, select a Philippines subsidiary.
    
3.  In the **Reports** field, select **Annual Alphalist of Payees (1604E)**.
    
4.  Select the tax period (fiscal year) for the report.
    
    Note:
    
    The fiscal year available starts from 2024 onwards.
    
5.  Select a tax type. Only tax types of the nexus associated with the subsidiary are available for selection.
    
6.  Click **Submit**.
    
7.  When the report is displayed, click any of the following options:
    
    -   **Print PDF**
        
    -   **Export - CSV**
        
    -   **Export - DAT**
        
    -   **Return to Criteria**
        

## Payment Form (0605) {#bridgehead_0224095554}

Use the Payment Form or Form 0605 for reporting and remitting taxes and fees that don't require a tax return. For example, BIR requires that you fill out Form 0605 when a tax payment or penalty is due, or to process an advance payment. Generally, you need this form for annual registration or processing assessment fees.

#### To generate Form 0605 reports: {#procedure_42095834276}

Tip:

After printing, click **Refresh** to view the latest generated report in the **Report History** subtab.

1.  Go to Reports > Withholding Tax > Withholding Tax Reports.
    
2.  Select a Philippines subsidiary in the **Subsidiary** field or select **Philippines** in the **Nexus** field.
    
3.  Select **Form 0605** in the **Reports** field.
    
4.  Select the relevant tax period in the **Tax Period** field.
    
    Important:
    
    Click **Refresh** each time you change the tax period (monthly, quarterly, or yearly).
    
5.  Enter values in the following manual input fields:
    
    -   For the Calendar or Fiscal Year
        
    -   Year Ended
        
    -   Quarter (leave blank if Calendar or Fiscal year is chosen)
        
    -   Due Date
        
    -   No. of Sheets Attached
        
    -   ATC
        
    -   Return Period
        
    -   Tax Type Code
        
    -   Background Information
        
    -   Taxpayer's Name
        
    -   Telephone Number
        
    -   Registered Address
        
    -   Zip Code
        
    -   Manner of Payment
        
    -   Type of Payment
        
    -   Computation of Tax amounts
        
    -   Signatory Details
        
    -   Details of Payment
        
6.  Click **Print** to download a PDF file of the report.
    
    The following footer information appears on the bottom right of every printed Form 0619-F:
    
    -   First line: Printed by `<user + user ID>` on `<date and time stamp>`
        
    -   Second line: Oracle NetSuite (edition) (version)
        

Use the **Report History** subtab to view a list of generated Form 0605 reports. You can download any of the reports individually and attach as a supplementary document for Form 1601-EQ or other reports.

#### To view and download Form 0605 reports: {#procedure_55100711392}

1.  Go to Reports > Withholding Tax > Withholding Tax Reports.
    
2.  Select a Philippines subsidiary in the **Subsidiary** field or select **Philippines** in the **Nexus** field.
    
3.  Select **Form 0605** in the **Reports** field.
    
4.  Click the **Report History** subtab to view a list of generated reports.
    
5.  Click the corresponding **Download** link to save a PDF in your designated folder (for example, `C:\Users[your name]\Downloads`). Check your browser settings to locate the download folder.
    
    Downloaded reports use the following naming convention: `[TIN][Form0605][TaxPeriod][PaymentType][DateGenerated].pdf`
    
    Where:
    
    -   `TIN` is the 9-digit Taxpayer Identification Number followed by the 3-digit branch code.
        
    -   `Form0605` is the form name.
        
    -   `TaxPeriod` is based on the Tax Period that you have selected.
        
    -   `PaymentType` is `AnnualFee`, `QuarterlyPayment`, or `MonthlyPayment`.
        
    -   `DateGenerated` is the date you submitted the payment, in YYYY-MM-DD format.
        
    
    For example: `12345678901234_0605_A2025_AnnualFee_2025-02-10.pdf`
    

## Summary Alphalist of Withholding Tax Agents/Payors of Income Payments subjected to Creditable Withholding Tax at Source (SAWT) {#bridgehead_N1967231}

The Summary Alphalist of Withholding Tax Agents/Payors of Income Payments subjected to Creditable Withholding Tax at Source (SAWT) is a consolidated alphabetical listing of withholding agents from whom income was earned or received, and subjected to withholding tax.

This list is submitted by the recipient of the income as an attachment to tax returns for a specified period. The list shows, among others, total amounts of income/gross sales/gross receipts, and claimed tax credits taken from all Certificates of Creditable Withholding Tax at Source (BIR Form No. 2307) issued by the income payors.

#### To generate a SAWT: {#procedure_N1967248}

1.  Go to Reports > Withholding Tax > Withholding Tax Reports.
    
2.  In the **Subsidiary** field, select a Philippines subsidiary.
    
3.  In the **Reports** field, select **Summary Alphalist of Withholding Taxes (SAWT)**.
    
4.  Select the tax period for the report.
    
5.  Select the tax type used for creditable withholding tax. Only tax types of the nexus associated with the subsidiary are available for selection.
    
6.  Click **Submit**.
    
7.  When the report is displayed, click any of the following options:
    
    -   **Print PDF**
        
    -   **Export - CSV**
        
    -   **Export - DAT**
        
    -   **Return to Criteria**
        

### Related Topics

-   [Accounting for Creditable Withholding Tax - Philippines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1960490.html)
-   [Setting Up Withholding Tax - Philippines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1960928.html)
-   [Creating Withholding Tax Types - Philippines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1961351.html)
-   [Creating Withholding Tax Codes - Philippines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1961532.html)
-   [Creditable Withholding Tax Codes - Philippines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1961761.html)
-   [Withholding Tax Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079416.html)
-   [Setting Up Withholding Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079716.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
