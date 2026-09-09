---
id: "section_N3535978"
type: "section"
title: "Troubleshooting PHP and SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services PHP Toolkit > Troubleshooting PHP and SOAP Web Services"
parent: "chapter_N3533866"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535978.html"
anchors: []
sha256: "717c886e0d63b99a535aad7d28d279cb57e7d41e3ee5d1015857fe5af2b99a7c"
---

The following table provides solutions for problems that may be encountered when using PHP with NetSuite's SOAP web services.

| Problem | Solution |
| --- | --- |
| The following error is returned when attempting to send requests over https: Fatal error: Uncaught SoapFault exception: \[WSDL\] SOAP-ERROR: Parsing WSDL: Couldn't load from 'https://webservices.netsuite.com/wsdl/v2017\_2\_0/netsuite.wsdl'. | Edit the php.ini file by uncommenting "extension=php\_openssl.dll" under Dynamic Extensions. Windows only: Make sure that libeay32.dll and ssleay32.dll files are in your path. You can do this by copying the files to your System32 folder. |
| The following time out error is returned: Fatal error: Maximum execution time of 30 seconds exceeded. | Edit the php.ini file and change max\_execution\_time - 30 (or default value) to 200. |
| The following error message is returned: Debug Error: Uncaught SoapFault exception: \[HTTP\] Error Fetching http headers. | Edit the php.ini file and by setting default\_socket\_timeout = 200. |
| The following error message is returned: Warning: It is not yet possible to assign complex types to properties. | Open the php.ini file and edit error\_reporting. Set it to E\_ERROR instead of E\_ALL. |
| The execution of script stops and error was not shown, or notices are being shown on the page. | Open the php.ini file and set error\_reporting = E\_ERROR & ~E\_NOTICE. |
| The following error is returned: Fatal error: Allowed memory size of 8388608 bytes exhausted (tried to allocate 3024 bytes). | Open the php.ini file and set memory\_limit = 80M. |
| Performance issue: Every time a SOAP web services request executes, PHP performs a GET on the wsdl. | For a non-Windows installation of PHP, look for property soap.wsdl\_cache\_dir in the php.ini file and make sure that the specified folder ("/tmp" -> c:\\tmp) exists in the host. Note: For a **Windows** installation of PHP, change the caching directory to something similar to: soap.wsdl\_cache\_dir="c:/Windows/Temp" Also, since a NetSuite WSDL version does not change after its release, you can increase the wsdl\_cache\_ttl to six months, until the release of the next WSDL version. This way you avoid downloading the WSDL multiple times, limiting the available room for errors and performance issues. |
| You have made a change in your php.ini file, yet the value you set is not respected. | Make sure that the property exists only one time in the php.ini file. |

### Related Topics

-   [PHP Toolkit Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534011.html)
-   [Downloading the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534718.html)
-   [Configuring an Environment for the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534858.html)
-   [Creating a SOAP Web Services PHP Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535140.html)
-   [Creating and Submitting Records Using the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535701.html)
-   [Logging SOAP Requests and Responses Using the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535863.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
