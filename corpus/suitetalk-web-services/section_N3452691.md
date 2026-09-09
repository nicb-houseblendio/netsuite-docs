---
id: "section_N3452691"
type: "section"
title: "Built-in Types"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Types > Built-in Types"
parent: "chapter_N3452524"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452691.html"
anchors: []
sha256: "bf1d5c1ee0ea714b36044ce6f58a07b01c542e36bca77a44942f89000e944d72"
---

Built-in (or primitive) types are those that are not defined in terms of other datatypes. They are used as a standardized way to define, send, receive and interpret basic data types in SOAP messages. Primitive data types used in the SOAP web services can be modified for display purposes. For example, although a price field may be passed in the SOAP messages using an integer primitive data type, the NetSuite UI may format the value with a currency symbol for display purposes.

Of the extensive set of built-in (or primitive) types provided by the XML Schema language specification, the SOAP web services implementation uses the following built-in types. For detailed information on XML Schema built-in types, refer to [http://www.w3.org/TR/xmlschema-2/](http://www.w3.org/TR/xmlschema-2/).

-   **string** -represents character strings in XML
    
-   **int** - derived from the decimal type and represents the standard concept of the integer numbers
    
-   **double** - is patterned after the IEEE double-precision 64-bit floating point type
    
-   **boolean** - represents the concept of binary-valued logic: {true, false}. In NetSuite, a boolean field can be set to true, false, 1 to indicate true, or 0 to indicate false.
    
    -   In the 2010.2 endpoint and later, SOAP web services validates boolean values. Each value must be a true xsd boolean (0,1,true,false) as per the W3C specification. For [details, see the specification](http://www.w3schools.com/schema/schema_dtypes_misc.asp).
        
    -   In endpoints prior to 2010.2, invalid values are treated as false.
        
-   **dateTime** - represents integer-valued year, month, day, hour and minute properties. For example, **2005-09-21T15:24:00.000-07:00**, where 2005-09-21 is the date, 15:24:00.000 is the time and -07:00 is the timezone offset. For more information about the dateTime type, see [Datetime Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1521451348.html).
    

### Related Topics

-   [Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3452524.html)
-   [Complex Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452954.html)
-   [Custom Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3458179.html)
-   [Search Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3460474.html)
-   [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
