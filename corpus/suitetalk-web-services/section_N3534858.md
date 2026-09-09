---
id: "section_N3534858"
type: "section"
title: "Configuring an Environment for the PHP Toolkit"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services PHP Toolkit > Configuring an Environment for the PHP Toolkit"
parent: "chapter_N3533866"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534858.html"
anchors: ["bridgehead_N3534910", "bridgehead_N3534967"]
sha256: "c8a4b95b4441d370f4dc4f7133046d830d4f6696e62f9b860d3035cbda65277b"
---

You can run PHP scripts from the command line by installing a PHP interpreter. Command line scripts are suitable for stand-alone applications and are useful for scripting and testing. See [Installing PHP for the Command Line](#bridgehead_N3534910) for more details.

The PHP Toolkit's real power, however, is in the ability to use a web server-based PHP interpreter module to integrate NetSuite into an existing web presence, whether it is an external e-commerce website, or an intranet-only Human Resources portal, for example.

A web server executes a PHP script through the included PHP interpreter module. PHP scripts can be text files containing PHP code, or they can be HTML web pages containing PHP tags indicating sections of PHP code. See [Installing a Web Server for PHP](#bridgehead_N3534967) for more details.

Note:

For information on downloading the PHP Toolkit, see [Downloading the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534718.html).

## Installing PHP for the Command Line {#bridgehead_N3534910}

Many distributions of Linux and macOS are pre-installed with PHP. Packages for Windows® can be obtained from [http://windows.php.net/download/](http://windows.php.net/download/).

After PHP is installed, you need to edit the php.ini file. The PHP Toolkit needs to use certain libraries that are not enabled in a PHP installation by default.

In the php.ini configuration file, in the section \[Dynamic Extensions\], the following lines need to be added if they do not exist:

          `extension=php_soap.dll extension=php_openssl.dll` 
        

The modules indicated by the .dll extensions pertains to a Windows installation. If you are configuring a Unix-based platform, change **.dll** to **.so**:

          `extension=php_soap.so extension=php_openssl.so` 
        

Note:

For a Windows installation of PHP, change the caching directory to something similar to:

soap.wsdl\_cache\_dir="c:/Windows/Temp"

## Installing a Web Server for PHP {#bridgehead_N3534967}

Note:

This section talks about using Apache Web Server, but any web server that supports PHP, SSL, and SOAP should be able to be used for SOAP web services.

The simplest way to provision a web server for the PHP Toolkit is to install a LAMP package. LAMP is the acronym for Linux, Apache, MySQL, and PHP. After a LAMP package is installed, a complete web server with database and PHP scripting functionality is available with little configuration required. The PHP Toolkit does require, however, that you make a few modifications to the default LAMP installation.

Note:

There are several LAMP distributions available free of charge for most computer architectures. A well known package for Windows® is WAMP, which is available at http://www.wampserver.com/en/. Follow the instructions that come with the package to install and initially configure it.

After LAMP is installed, the php.ini and the httpd.conf configuration files need to be edited. Note that the LAMP installation will not use any existing PHP installation; it will install its own self-contained PHP package.

In the php.ini configuration file, in the section \[Dynamic Extensions\], the following lines need to be added if they do not exist:

          `extension=php_soap.dll extension=php_openssl.dll` 
        

The modules indicated by the .dll extensions pertains to a Windows installation. If you are configuring a Unix-based platform, change **.dll** to **.so** :

          `extension=php_soap.so extension=php_openssl.so` 
        

The Apache Web Server needs to be told to load the PHP module so that it can run PHP scripts. In the httpd.conf configuration file in the section Dynamic Shared Object Support, the following line must be added. (Note that the line may already exist; in that case check that the path to the PHP module is correct.)

          `LoadModule php5_module  C:\<PATH TO PHP>\modules\libphp5.dll` 
        

The module indicated by the .dll extension pertains to a windows installation. If you are configuring a Unix-based platform, the PHP module will have a **.so** extension. Note also that the path to the PHP module will differ:

          `LoadModule php5_module  /<PATH TO PHP>/bin/php/modules/libphp5.so` 
        

Important:

As indicated in these examples, the name of the module is libphp5.dll or libphp5.so, but be aware that SOAP web services requires PHP 5.**6** or later. In other words, the name of the module is not specific to the exact PHP version. (However, the exact version is likely indicated by the <PATH TO PHP> folder name.)

Important:

After a change to any configuration files, LAMP's services must be restarted.

Important:

If you are running PHP scripts from the command line **and** through a web server, there will be **two** php.ini files that need to be edited, one for the command line PHP installation, and one provided by the LAMP installation.

Note:

For a Windows installation of PHP, change the caching directory to something similar to:

soap.wsdl\_cache\_dir="c:/Windows/Temp"

### Related Topics

-   [PHP Toolkit Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534011.html)
-   [Downloading the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534718.html)
-   [Creating a SOAP Web Services PHP Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535140.html)
-   [Creating and Submitting Records Using the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535701.html)
-   [Logging SOAP Requests and Responses Using the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535863.html)
-   [Troubleshooting PHP and SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535978.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
