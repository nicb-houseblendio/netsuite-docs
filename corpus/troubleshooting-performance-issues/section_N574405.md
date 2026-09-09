---
id: "section_N574405"
type: "section"
title: "Troubleshooting Client Performance"
branch: "troubleshooting-performance-issues"
category: "performance"
breadcrumb: "Performance > Troubleshooting Performance Issues > Troubleshooting Client Performance"
parent: "chapter_4381204850"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N574405.html"
anchors: ["subsect_162152224029", "procedure_N574433", "subsect_162152239723", "procedure_N574477"]
sha256: "1cff8afcdd995343c2665a9aa848ea1ef69eb79334ce2e691af078d45b7b6175"
---

Client performance refers to how long it takes for your computer to display a page. Other applications running on your computer, in addition to NetSuite, are using your computer's resources. These applications may impact the performance of the NetSuite application on your computer.

You might notice client performance issues in one browser but not another. For example, some browsers may render pages faster than others. These differences may result from browser configuration, security defenders, and individual browser add-ons. For more details, see [Supported Browsers for NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N340018.html).

Also note that some NetSuite tasks require intensive resources (for example, creating a sales order with 200 items).

If you notice client performance issues, the following procedures can help you identify and troubleshoot them.

## Identifying Client Performance Issues {#subsect_162152224029}

Use the following steps to identify client performance issues.

#### To identify client performance issues: {#procedure_N574433}

There are no universal requirements for the amount of RAM a computer must have or how fast it must be to run NetSuite. The requirements depend on how you're using your computer and the other applications running on it. For example, your computer may be able to run NetSuite but may not be powerful enough to run NetSuite with your Voice Over Internet Protocol (VoIP) application. Or, your computer is powerful enough to run your VoIP application and NetSuite at the same time, but it cannot create a sales order that contains 200 line items.

1.  On your computer, open the Task Manager.
    
2.  Click the **Processes** tab.
    
3.  Click **Memory** to sort the processes based on memory usage, or RAM.
    

## Troubleshooting Client Performance Issues {#subsect_162152239723}

Use the following steps to troubleshoot client performance issues.

#### To troubleshoot client performance issues: {#procedure_N574477}

1.  Close all the applications you're not using. If you need to run more than one application, consider increasing your computer resources (RAM).
    
2.  Check your firewall application or other threat detection software. Some of these applications check the page before loading it in your browser, which can cause a delay. Adding a new rule to explicitly allow traffic from and to \*.netsuite.com domains may reduce latency. For more information, see [NetSuite IP Addresses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N251955.html), or consult the documentation of your firewall or threat protection software provider.
    
3.  Remove any spyware that could be using your computer's resources.
    
4.  Determine whether the issue is only happening for one type of form. Try to determine what is different about the form compared to other forms that load more quickly.
    
5.  Test using different browsers. Use the browser that displays the page faster.
    
6.  Determine whether there are add-ons running in your browser, such as antivirus add-ons, anti-spam add-ons, or phishing add-ons. Eliminate browser add-ons, one by one, to identify the cause of the issue.
    

### Related Topics

-   [Application Performance Management (APM)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4283522055.html)
-   [Optimizing NetSuite Performance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N571805.html)
-   [Performance Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_2111656357.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
