---
id: "section_N3445354"
type: "section"
title: "Monitoring Asynchronous Jobs from the UI"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Processing > Asynchronous Request Processing > Monitoring Asynchronous Jobs from the UI"
parent: "section_3770809638"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3445354.html"
anchors: ["bridgehead_3812613361", "bridgehead_3812614851"]
sha256: "3ff92572f14f918adb2a5654858ddb0c708184f2319120df394b0d2d93b3d433"
---

SOAP web services jobs submitted asynchronously can be monitored at _Setup > Integration > SOAP Web Services Process Status_. To access this log, either the full SOAP Web Services permission or the View SOAP Web Services Logs permission is needed. Both permissions are available on the role record's Permissions subtab under Setup.

On this page, you can view the following information about each job:

-   Date - the date the job was created
    
-   Sequence - the order of the job in relation to other asynchronous jobs in process (jobs are processed on a first in, first out basis)
    
-   Job Number - order number of the job in the work queue
    
-   Job Id - the Job Id, which is also returned in the asynch SOAP response, and can be used to programmatically retrieve job status information
    
-   Status - the status of the job: failed, finishedWithErrors, pending, processing, or finished (for more on status, see [Checking the Status of an Asynchronous Job](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3771741984.html))
    
-   Percent Complete - the percentage of job processing that has been completed
    
-   Est. Remaining Time - the estimated amount of time remaining before the job is completed
    
-   Request - the SOAP request associated with the job (see additional details below)
    
-   Response - the SOAP response associated with the job (see additional details below)
    
-   Cancel - you can check the box in this column to cancel a job that has not yet successfully completed
    

## Limits on Requests and Responses {#bridgehead_3812613361}

Note the following limitations:

-   A response for a job is available only after the job has successfully completed.
    
-   In production environments, the data is accessible for 21 days. In sandbox environments, the data is accessible for seven days.
    
-   Lengthy requests and responses are not saved by the system and therefore are not available for your review. The system imposes the following limits:
    
    -   The system does not save requests that are larger than 100MB.
        
    -   The system does not save responses that are large than 1MB.
        

## Refreshing the Job Status Page {#bridgehead_3812614851}

The Job Status page does not automatically refresh. To get the current status of a job, click the Refresh button at the top of the page.

### Related Topics

-   [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html)
-   [Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770809638.html)
-   [Checking the Status of an Asynchronous Job](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3771741984.html)
-   [Checking for Detailed Results of an Asynchronous Job](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3771740553.html)
-   [Synchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444684.html)
-   [Using the SOAP Web Services Usage Log](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444819.html)
-   [Creating Integration Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3445008.html)
-   [SOAP Web Services Governance Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418637.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
