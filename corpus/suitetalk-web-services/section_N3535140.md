---
id: "section_N3535140"
type: "section"
title: "Creating a SOAP Web Services PHP Project"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services PHP Toolkit > Creating a SOAP Web Services PHP Project"
parent: "chapter_N3533866"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535140.html"
anchors: []
sha256: "bc382d86b735e949ae0a8c2298c6f2fcec8a00542e57487997da95ab7a5beb4c"
---

For each project you need to perform the following steps:

1.  Copy the PHPToolkit directory to the directory in your IDE where your project resides.
    
2.  Edit the NSconfig.php file, substituting your own account details.
    
3.  If SOAP logging is required, create a folder called **nslog** inside the PHPToolkit folder. See [Logging SOAP Requests and Responses Using the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535863.html) for more details.
    
4.  Each solution needs to include the NetSuiteService.php file by adding the following line to the main source file:
    
                  `require_once '../PHPToolkit/NetSuiteService.php';` 
                
    
    This step will prompt most IDEs to parse the NetSuiteService.php file for auto completion information.
    
5.  Instantiate a service:
    

          `$service = new NetSuiteService();` 
        

Important:

Each time you upgrade your NetSuite endpoint, for example from WSDL version 2023.2 to 2025.2, you will also need upgrade the NetSuiteService.php class library to take advantage of any new features.

In 2016.1, token-based authentication support was added to the PHPToolkit.

The following guidelines should be followed when using token-based authentication with PHPToolkit:

-   Each request requires a unique TokenPassport
    
-   NetSuite does not generate TokenPassports. You must provide your own implementation of iTokenPassportGenerator
    
-   You configure NetSuite to use your iTokenPassportGenerator by calling the setTokenGenerator:
    
                  `$generator = new MyTokenPassportGenerator(); $service->setTokenGenerator($generator);` 
                
    

For more information about token-based authentication, see [Token-based Authentication (TBA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4247329078.html).

### Related Topics

-   [PHP Toolkit Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534011.html)
-   [Downloading the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534718.html)
-   [Configuring an Environment for the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534858.html)
-   [Creating and Submitting Records Using the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535701.html)
-   [Logging SOAP Requests and Responses Using the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535863.html)
-   [Troubleshooting PHP and SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535978.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
