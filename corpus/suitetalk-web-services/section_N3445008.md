---
id: "section_N3445008"
type: "section"
title: "Creating Integration Reports"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Processing > Synchronous Request Processing > Creating Integration Reports"
parent: "section_N3444684"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3445008.html"
anchors: ["bridgehead_N3445108", "bridgehead_N3445150", "bridgehead_N3445185", "procedure_N3445198"]
sha256: "52498fbee578465df86eb0598df5432efef1b985976c3227662cd61fcc922f2e"
---

You can monitor SOAP web services processing by creating the following types of integration reports:

-   [Integration and Automation Usage Summary by Job](#bridgehead_N3445108)
    
-   [Integration and Automation Usage Summary by Record Type](#bridgehead_N3445150)
    

Important:

The **Integration** permission is required to view these reports. To enable this permission, administrators must go to _Setup > Users/Roles > Manage Roles_. Click Customize next to the appropriate role. On the Permissions subtab, click Reports. In the Permissions dropdown list, select **Integration** and click Add.

Note:

You might receive a timeout error when creating integration reports for accounts with large volumes of SOAP web services traffic. Also, although integration reports do offer some filtering capabilities, users must first take the added step of customizing the report. Be aware that you can apply filtering in the SOAP Web Services Usage Log without doing customization.

Both of these reports provide details on type of operations used (for example, add, addList, delete), who performed an operation, and the time an operation was performed.

Web Services Integration reports are also useful for administrators who need to diagnose and troubleshoot issues. Note that each report can be customized to display only the desired information. To customize a report, click Customize next to the desired report and then modify the report as desired. For details about how to customize a report, see the help topic [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html).

If an integration report is timing out, you should customize the report by adding filters so the report returns fewer results. See [Filtering Integration Report Data](#bridgehead_N3445185).

Note:

These reports do not support reporting by period even when the Report by Period preference is set to All Reports. The Report by Period preference can be configured at _Home > Set Preferences_, the Analytics subtab.

## Integration and Automation Usage Summary by Job {#bridgehead_N3445108}

This report can be used for performance statistics. It shows the duration of each SOAP web services processing job, the number of records modified in each job, the number of successful versus failed record modifications for each job, and the number of records queried for each job. You can also drill down to job details by clicking the job number.

Any related SOAP files are stored in View links in the reports Request Doc and Response Doc columns. Be aware that NetSuite purges SOAP files every 30 days. In sandbox environments, these files are accessible for seven days.

Note:

In sandbox environments, you can view request and response information in log and search results after 7 days. However, links to the original SOAP request and responses are not available.

You can view this report at _Reports > Integration > Integration and Automation Usage Summary by Job_.

## Integration and Automation Usage Summary by Record Type {#bridgehead_N3445150}

This report lists the record types modified by SOAP web services processing, and the number of records added, updated, deleted, and queried for each record type.

You can view this report at _Reports > Integration > Integration and Automation Usage Summary by Record Type_.

## Filtering Integration Report Data {#bridgehead_N3445185}

You can customize integration reports to run faster, by adding filters that limit the returned results. For example, you could limit a report to return only jobs with start dates that fall into a specified date range.

#### To filter an integration report by start date: {#procedure_N3445198}

1.  Go to _Reports > Integration > Integration and Automation Usage Summary by Job > Customize_ or _Reports > Integration > Integration and Automation Usage Summary by Record Type > Customize_.
    
2.  Click **Filters**.
    
3.  Under **Search Fields** box, enter **Start Date** and click the **Search** button.
    
    The **Actual Job Start Date** and **Start Date** fields are listed.
    
4.  Click **Start Date**.
    
    This field is added to the **Choose Filters** pane.
    
5.  In the **Choose Filters** pane:
    
    1.  Set **Filter** to between.
        
    2.  Set **Date Range** to custom.
        
    3.  In the **From** and **To** fields, enter dates in {mm/dd/yyyy} format.
        
    4.  Click **Done**.
        
6.  Click **Save**.
    

### Related Topics

-   [Synchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444684.html)
-   [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html)
-   [Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770809638.html)
-   [Using the SOAP Web Services Usage Log](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444819.html)
-   [Handling of Lengthy Requests](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4078474279.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
