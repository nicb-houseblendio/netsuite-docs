---
id: "section_N2031770"
type: "section"
title: "Viewing the VAT100 Submission History"
branch: "united-kingdom-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > United Kingdom Help Topics > United Kingdom Tax Topics For Accounts Without SuiteTax > United Kingdom VAT100 Tax Report > Viewing the VAT100 Submission History"
parent: "section_N2029877"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2031770.html"
anchors: ["procedure_N2031801"]
sha256: "7192ff70d3f0c6a6e303128f2311bde08679369c688722f4079211a8cb381bfe"
---

Important:

Beginning April 8, 2021, HMRC no longer accepts non-MTD VAT submissions. Refer to [Making Tax Digital for VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543299566.html) for the complete information of U.K.'s VAT direct filing solution.

You can view the submission history of your VAT100 reports by clicking the System Notes tab on the VAT form.

Warning:

If you remove the International Tax Reports SuiteApp from your account, the VAT submission history is deleted and cannot be recovered.

#### To view the VAT100 submission history: {#procedure_N2031801}

1.  Go to Reports > VAT/GST > Tax Reports (International).
    
2.  On the Tax Reports page, select the United Kingdom VAT registered subsidiary for which you want to see the United Kingdom VAT100 submission history.
    
3.  Select the **United Kingdom** country form.
    
4.  When the VAT100 tax form is displayed, click the **System Notes** tab.
    
5.  Review the information in the following columns:
    
    -   **User Name** - name of the user who filed the VAT return
        
    -   **Date** - date of submission
        
    -   **Status** - submission status
        
    -   **From Period** - tax period start date on the VAT report
        
    -   **To Period** - tax period end date on the VAT report
        
    -   **View** - link to open the VAT Online Submitted Period record in NetSuite
        
6.  Click the **Open** link of the submission record that you want to view. The **VAT Online Submitted Periods** record displays the following information:
    
    -   **Tax Period** - tax period on the VAT return
        
    -   **Subsidiary** - name of the subsidiary company
        
    -   **Status** - submission status
        
        -   **Success** means that the full submission was accepted by HMRC. This status is indicated by the Submit and Save button being dimmed on the VAT100 form, which means you cannot click the button.
            
            This status doesn't necessarily mean that all line items were correct. For example, you may determine that one or more of the amounts you submitted were in error or you may see a failed line item upon review of the Response field when you view the VAT100 submission history.
            
            **Next Steps:** In this situation, you can fix the errors and submit the corrected lines in the VAT100 report for the next tax period. Go to the HMRC Web site for more guidelines on what to do to correct mistakes.
            
        -   **Failure** means that the entire submission isn't accepted by HMRC for any reason. This situation can occur if HMRC online becomes unavailable or there is another type of transmission failure.
            
            **Next Steps:** In this situation, you have to fix the errors, run the report again, and resubmit it.
            
    -   **Submit User** - name of the user who submitted the report
        
    -   **Submit Date** - date of submission to HMRC
        
    -   **Request tab** - the request sent to HMRC in XML format
        
    -   **Response tab** - the response received from HMRC in XML format
        
        The response provides detailed messages about the success or failure of the submission, including error messages. A submission receipt reference is also displayed if the submission was accepted.
        
    -   **Folder Name** - name of the File Cabinet folder where successfully submitted reports are stored in PDF format. Fore more information, see [Viewing the Submitted VAT100 in the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2032419.html).
        
7.  Review the response information in detail, whether the submission failed or succeeded, to determine if you need to resubmit all or part of the VAT100 report. For more information, see [Errors in your VAT100 Submission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2032238.html).
    

Important:

You cannot resubmit the VAT100 report for the same period. If you need to fix the line items that were incorrect or unsuccessful during this submission, you must include them in the report for the subsequent tax period.

### Related Topics:

-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Setting Up Tax Filing for United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2029554.html)
-   [United Kingdom VAT100 Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2029998.html)
-   [What goes into each box - United Kingdom VAT100 report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2030237.html)
-   [Generating a United Kingdom VAT100 Tax Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2031051.html)
-   [Making Tax Digital for VAT](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543299566.html)
-   [Making Tax Digital for VAT Overview and Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543833477.html)
-   [Submitting MTD VAT Returns to HMRC](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543833633.html)
-   [Submitting an MTD VAT Return in a CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1547520822.html)
-   [Viewing Submission History of United Kingdom MTD CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1558408249.html)
-   [Viewing Previously Submitted MTD VAT Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543833722.html)
-   [Viewing the MTD VAT Return Submission History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543833748.html)
-   [Handling MTD VAT Return Submission Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156385546699.html)
-   [Exporting a United Kingdom VAT Return to Excel](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543833696.html)
-   [Sending of MTD Anti-Fraud Headers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161597724226.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
