---
id: "section_N3420833"
type: "section"
title: "Building an Application with Java using Apache Axis"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Setup > SOAP Web Services Quick Start > Building an Application with Java using Apache Axis"
parent: "section_N3419782"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3420833.html"
anchors: ["procedure_N3420861"]
sha256: "959cda73c2f43ba0af1743e4f9a97ed3c405be8a9135940909fdc016d61eef13"
---

Learn how to build a SOAP web services application using Apache Axis (versions 1.3 and 1.4) in this section.

Note:

The Java sample application available provides an in-depth look at how to build an application using Apache Axis and NetSuite SOAP web services. See [Downloading Sample Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421207.html) for more information.

#### To use the Apache Axis framework with NetSuite SOAP web services: {#procedure_N3420861}

1.  Install Java JDK 8.
    
    Download and install Java JDK 8. Ensure that the executables are available through the system path. This is required because all inbound and outbound secure communication must use TLS 1.2 or TLS 1.3.
    
2.  Install Apache Axis.
    
    1.  Download and install Apache Axis from [http://ws.apache.org/axis/](http://ws.apache.org/axis/).
        
        Important:
        
        The instructions work only for Axis version 1.4.
        
    2.  Download and install the Apache Axis patch for cookie management from NetSuite: [https://content.netsuite.com/download/axis1\_4\_patch.zip](https://content.netsuite.com/download/axis1_4_patch.zip)
        
        The NetSuite Web service implementation requires the client application to support multiple cookies on one line, as is the standard for cookies. There is a bug in Apache Axis that puts each cookie on its own line in the HTTP Headers. The patch version of the axis.jar fixes this problem. After the download is finished, replace the existing axis.jar file in your Axis root directory's lib folder with this version.
        
    3.  After installation, set an environment variable called AXIS\_HOME to point to the Axis installation directory.
        
3.  Install Apache Ant (Optional).
    
    Download and install Apache Ant, version 1.5 or higher, from [http://ant.apache.org/](http://ant.apache.org/). Apache Ant is a Java-based build tool that facilitates automation of the build process, including generating the proxy classes from the NetSuite WSDL.
    
    See the build.xml file in the Java sample application for a complete Ant build script.
    
4.  Configure Java to generate unreferenced types.
    
    Set the **all** parameter in your axis-wsdl2java ant task to **true**. For example:
    
                    `<axis-wsdl2java timeout="360000" output="${generated.src.dir}" verbose="true"        url="${wsdl-1.3.url}" all="true" wrapArrays="true">` 
                  
    
5.  Use Apache Ant to automatically generate the client proxy code.
    
    **Using Apache Axis from the command line**
    
    Use the WSDL2Java utility to generate the proxy classes as follows:
    
                    `java -cp <classpath> org.apache.axis.wsdl.WSDL2Java  -a -w -O 360000 <url>` 
                  
    
    Where the <classpath> points to the appropriate Apache Axis JAR files and <url> is the URL for the NetSuite WSDL.
    
    For example, the following commands will set the class path and generate the proxy classes:
    
                    `>set             CP=%AXIS_HOME%\lib\axis.jar;%AXIS_HOME%\lib\jaxrpc.jar;%             AXIS_HOME%\lib\commons-discovery.jar;%AXIS_HOME%\lib\wsdl4j.jar;             %AXIS_HOME%\lib\saaj.jar;>java -cp %CP% org.apache.axis.wsdl.WSDL2Java              https://webservices.netsuite.com/wsdl/v2017_1_0/netsuite.wsdl` 
                  
    
    **Using the Apache Axis task in Apache Ant**
    
    Create a build target that uses the WSDL2Java Ant task as follows where the ${generated.src.dir} variable is the directory where the source code is generated and the ${wsdl.url}variable points to the NetSuite WSDL.
    
                    `<target name="generate.interfaces" description="Generates              client interfaces using Axis">             <echo>Generating client interfaces using Apache Axis</echo>             <axis-wsdl2java output="${generated.src.dir}" verbose="true"              url="${wsdl.url}">             <mapping namespace="http://axis.apache.org/ns/interop"              package="interop"></mapping>             </axis-wsdl2java>             </target>` 
                  
    
6.  Ensure that the Ant executables are available on the system path. Run the Ant task as follows:
    
                    `ant generate.interfaces` 
                  
    
7.  Implement your application by writing your business logic using the generated axis proxy classes.
    
    1.  Locate the NetSuite service.
        
                            `NetSuiteServiceLocator service = new NetSuiteServiceLocator();` 
                          
        
    2.  Enable support for multiple cookie management.
        
                            `service.setMaintainSession( true );` 
                          
        
    3.  Get the NetSuite port.
        
                            `NetSuitePortType port = service.getNetSuitePort();` 
                          
        
    4.  Create a valid session by populating the Passport object and then invoking the login operation.
        
                            `passport.setEmail( "username@netsuite.com" );             passport.setPassword( "<SOAP web services password>" );             role.setid( "3" );             passport.setRole( role );             passport.setAccount( "TSTDRV96" );             Status status = port.login( passport ).getStatus();` 
                          
        
    5.  Implement your business logic. For example, create a new customer in NetSuite.
        
                            `Customer cust = new Customer();             cust.setEntityID( 'XYZ Inc' );             WriteResponse response = port.add( cust );` 
                          
        
    6.  Log out to invalidate the current session.
        
                            `port.logout();` 
                          
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Quick Start](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3419782.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [Enabling the SOAP Web Services Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3419926.html)
-   [Setting the Show Internal IDs Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3420345.html)
-   [Downloading Sample Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421207.html)
-   [Capturing SOAP](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421282.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
