---
id: "section_N3421207"
type: "section"
title: "Downloading Sample Applications"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Setup > SOAP Web Services Quick Start > Downloading Sample Applications"
parent: "section_N3419782"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421207.html"
anchors: ["subsect_97145049637", "subsect_44145942810"]
sha256: "78abf9f67e03841999d598a31141fef323c99488653d38e91a70cf9335bc8058"
---

To familiarize yourself with NetSuite web services, we encourage you to download our sample Java application. This command-line application demonstrates some of the key platform features.

The Java sample application require version 1.4 or higher of the Apache Axis framework and a NetSuite [patch](https://content.netsuite.com/download/axis1_4_patch.zip) for cookie management (please see the NetSuite Help Center for details).

SOAP web services developers can download sample applications from the link:

[Download Java - Apache Axis sample application](https://content.netsuite.com/download/NSJavaClient2025-2.zip)

## PHP Toolkit {#subsect_97145049637}

The PHP toolkit simplifies the process of developing integrations that use PHP 5.6 or later. The toolkit enables auto-completion in major IDEs for records, fields, operations, and arguments. This makes PHP programming with SuiteTalk faster and less error prone. The toolkit supports all SOAP web services operations. The toolkit also includes a sample application modeled after a typical e-commerce integration.

1.  Download the toolkit [PHP\_Toolkit\_2025\_2](https://content.netsuite.com/download/PHPToolkit_2025_2.zip) file.
    
2.  Unzip the file and save the toolkit files to the project folder in your IDE.
    
3.  Start using the toolkit by adding a `require_once` statement. For example:
    
    `require_once 'PHPToolkit/NetSuiteService.php';`
    
4.  Configure the connection parameters such as server, email, and password by modifying the defaults in the NSconfig.php file.
    
5.  In the php.ini configuration file, in the section \[Dynamic Extensions\], add the following lines, if they do not already exist:
    
    `extension=php_soap.dll`
    
    `extension=php_openss.dll`
    

Note:

If you are configuring the PHP Toolkit to run on a Unix-based platform, change the Windows `.dll` extension to a `.so` extension.

For a Windows installation of PHP, change the caching directory to something similar to: `soap.wsdl_cache_dir="c:/Windows/Temp"`

SOAP messages are logged in the PHPToolkit/nslog directory. If you do not want the messages logged, delete the directory.

For more information about the PHP toolkit, see [SOAP Web Services PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3533866.html).

## Sample Files for REST Web Services {#subsect_44145942810}

To familiarize yourself with REST web services, you can download a Postman environment template and a Postman sample request collection. These resources show you how to set up your NetSuite integration and send REST requests.

For information about downloading and using the Postman environment template and samples, see [Using Postman with REST Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1544794192.html).

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Quick Start](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3419782.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [Enabling the SOAP Web Services Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3419926.html)
-   [Setting the Show Internal IDs Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3420345.html)
-   [Building an Application with Java using Apache Axis](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3420833.html)
-   [Capturing SOAP](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421282.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
