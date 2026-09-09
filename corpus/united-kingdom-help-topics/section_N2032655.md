---
id: "section_N2032655"
type: "section"
title: "Viewing an EU Sales List (ESL) Report for the United Kingdom"
branch: "united-kingdom-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > United Kingdom Help Topics > United Kingdom Tax Topics For Accounts Without SuiteTax > EU Sales List for United Kingdom > Viewing an EU Sales List (ESL) Report for the United Kingdom"
parent: "section_N2032559"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2032655.html"
anchors: ["procedure_N2032710"]
sha256: "71579457b3bc28415788344a991311cae430e0f659c405966bdc7027cb8129c1"
---

Note:

This topic is for NetSuite accounts that use the EU Sales List Report page to generate the EU Sales List. If you are using the Country Tax Report page, see [EC Sales List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_156888850442.html).

Effective January 1, 2021, businesses located in Great Britain are no longer required to submit EU Sales List. However, it is still required for businesses located in Northern Ireland.

This feature requires the International Tax Reports SuiteApp (bundle ID 43003).

-   Make sure that each customer record has a VAT number in the appropriate format for the customer's country. You must also verify that the VAT numbers are valid on the current date by clicking the VIES link on the Financial tab of the customer record. If there is no VAT number specified on a subcustomer record, NetSuite will get the parent customer's VAT number.
    
    Each EU country has its own VAT prefix and numbering format. For information, refer to this [VAT identification number structure](http://ec.europa.eu/taxation_customs/vies/faqvies.do) published by the European Commission.
    
-   Make sure that each customer record has a shipping address. If there is no shipping address, then NetSuite will get the billing address saved on the customer record. If the invoice is charged to a project, then NetSuite will get the address saved on the customer record that the project is associated with.
    

Follow the steps for [United Kingdom EU Sales List (ESL) Online Filing Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2029554.html#bridgehead_4404016733) if you want to submit your ESL reports online directly from NetSuite to His Majesty's Revenue and Customs (HMRC). For more information, see [Setting Up Tax Filing for United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2029554.html).

#### To view an EU Sales List Report for the United Kingdom: {#procedure_N2032710}

1.  Go to Reports > VAT/GST > EU Sales List Report.
    
2.  Select a subsidiary. Be sure that you have already completed the EU sales filing setup for that subsidiary. See [Setting Up Tax Filing for United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2029554.html).
    
3.  Check the **Group** box if you want a consolidated report that includes child subsidiaries. Use this for companies that are part of a VAT group.
    
4.  Select a country form.
    
5.  Select a reporting period by entering the **Tax Period** From and To dates. You can select a month or a quarter.
    
6.  To display the report, click **Refresh**.
    
    Important:
    
    Click **Refresh** each time you change the reporting criteria (tax period).
    
7.  Carefully review the report. Be sure to check all pages of the report. The following information is displayed:
    
    -   **Customer** - Click the customer name to view the customer record.
        
    -   **Country** - Country code prefix of the customer's VAT registration number
        
    -   **Customer VAT Registration Number** - Customer's VAT number without the country prefix
        
    -   **Total Value of Supplies in Pounds Sterling** - Displayed in the appropriate format for United Kingdom
        
        Note:
        
        Values displayed are rounded down to the nearest whole pound.
        
    -   **Indicator** - Editable field that specifies if the transaction is for goods, services, or triangulation
        
8.  Verify and correct data as necessary. Any inconsistencies that NetSuite finds in your data, based on your selected reporting criteria, are indicated by color codes on the ESL report. By default, the system checks the **Exclude** box for those transactions with data inconsistencies, except for VAT number errors.
    
    ![Screenshot of EU Sales List legend](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/CountrySpecificFeatures/EUSalesListLegend.png)
    
    | Code | Definition |
    | --- | --- |
    | Customer is in same country | If the customer name is red, it means that the country of the EU Sales List form and the country on the customer's transaction record are the same. Make sure that you have used the correct shipping country on the transaction. |
    | Non-EU country transaction | If the customer name is brown, it means that the country in the shipping address of the transaction record isn't an EU country. Make sure that you have used the correct shipping country on the transaction. |
    | Customer without valid VAT ID/shipping address | If customer name is blue, it means that there is no identified shipping or billing address on the customer's transaction record. If VAT number is blue, it could mean that the VAT country code doesn't match the country indicated on the shipping address, or it could mean that the VAT number isn't in the correct format for that country. |
    
    Note:
    
    Each EU country has its own VAT prefix and numbering format. For information, refer to this [VAT identification number structure](http://ec.europa.eu/taxation_customs/vies/faqvies.do) published by the European Commission.
    
9.  Check the **Exclude** box for lines that you want to omit from your report, or clear any checked boxes for lines that you want to include in the report. Check the box in the column header to exclude all lines on the current page.
    
10.  Review the transaction type in the **Indicator** column for each line, and edit it if necessary:
     
     -   **B2B Goods** - products that you deliver directly to a customer
         
     -   **Triangulated Goods** - sales that involve supplies of goods between three VAT-registered traders in three different EU member states. This is the default indicator for transactions that you marked as part of an EU triangulation deal. For more information, see [Identifying EU Triangulated Goods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4380703631.html).
         
     -   **Services** - services that you provided to your customer
         
     
     Important:
     
     You should review all the values in the report prior to submission.
     
11.  To save the report, click any of the following options:
     
     -   **Print** - to print or save a PDF version of the report for your own records. Lines with the **Exclude** box checked are not included in the PDF.
         
     -   **Export** - to save the ESL report as a Microsoft Excel (.xls) file. Lines with the **Exclude** box checked are not include in the .xls file.
         
         Note:
         
         NetSuite also saves a copy of the file in the File Cabinet, and sends you an email containing a URL of the file location. The file size limit is 5 MB, and the File Cabinet storage limit is 10 GB.
         
     -   **Export (HMRC)** - converts the ESL into a CSV file that complies with the format required by the United Kingdom tax agency (HMRC). When asked to open or save the file, click Save File. Opening the file in Microsoft Excel causes the format to change, which results in errors in your submission. Save the file first, and if you need to open it, use a text editor such as Notepad.
         
     -   **Submit Online** - submits the EU sales list directly to the United Kingdom tax agency (HMRC).
         

For more information, read the following topics:

-   [Viewing the ESL Submission History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2034719.html)
    
-   [Errors in your ESL Submission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2034958.html)
    
-   [Viewing the Submitted United Kingdom ESL](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2035141.html)
    

### Related Topics:

-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Setting Up Tax Filing for United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2029554.html)
-   [EU Sales List Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2068226.html)
-   [Submitting an EU Sales List (ESL) Online in the United Kingdom to HMRC](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2034464.html)
-   [Viewing the ESL Submission History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2034719.html)
-   [Errors in your ESL Submission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2034958.html)
-   [Viewing the Submitted United Kingdom ESL](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2035141.html)
-   [Creating or Customizing Roles to Use the International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054151.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
