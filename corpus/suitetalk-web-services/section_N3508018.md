---
id: "section_N3508018"
type: "section"
title: "getServerTime"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > getServerTime"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508018.html"
anchors: ["bridgehead_N3508052", "bridgehead_N3508064", "bridgehead_N3508179", "bridgehead_N3508331", "bridgehead_N3508392", "bridgehead_N3508401"]
sha256: "e052867bd0feaef3f4f4dd31ee6e14db53eede5cbf50421c9e6a0eacb74c2a8b"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

This operation takes no arguments and returns the NetSuite server time in GMT, regardless of a user's time zone. Developers do not have to rely on client time when writing synchronization procedures because the client time may not be in synch with the NetSuite server time.

If you choose, you can write client code that takes the GMT returned by NetSuite and convert the time to your local time zone. The format of the dateTime value returned by getServerTime contains integer-valued year, month, day, hour and minute properties, a decimal-valued second property and a boolean time-zoned property (timestamp) - for example, 2005-09-21T15:24:00.000-07:00, where 2005-09-21 is the date, 15:24:00.000 is the time and -07:00 is your own time zone offset, if you choose to set one.

Any user can call getServerTime. There are no explicit permissions for this operation. For example, if you need to synchronize customer data with NetSuite, you can call getServerTime to initialize your synchronization process. To synchronize new or changed customers records, you can search customers and filter by **lastModifiedDate** using the value returned in getServerTime. To synchronize deleted customer records, you can call the [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) operation and use the value returned in getServerTime. This makes your synchronization process independent of your client time, which may not be in sync with the NetSuite server time and the timestamp we use to track changes.

## Request {#bridgehead_N3508052}

The GetServerTimeRequest type is used for the request. It takes no arguments.

## Response {#bridgehead_N3508064}

The GetServerTimeResponse type is used for the response. It contains the following elements.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| response | GetServerTimeResult | See GetServerTimeResult, below. |

## GetServerTimeResult {#bridgehead_N3508179}

The GetServerTimeResult type contains the following elements.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this request. All applicable errors or warnings will be listed within this type, which is defined in the platformCore XSD. |
| serverTime | dateTime | dateTime value returned is in GMT. |

## Faults {#bridgehead_N3508331}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3508392}

## Java {#bridgehead_N3508401}

          `public void testGetServerTime() throws Exception {    c.login();      GetServerTimeResult rs = c.getPort().getServerTime();    System.out.println("Welcome to NetSuite. At the sound of the tone the NetSuite time will be : " + new    SimpleDateFormat("yyyy-MM-dd HH:mm:ss").format(rs.getServerTime().getTime()));     System.out.println("This compares with a client time of " + new SimpleDateFormat("yyyy-MM-dd    HH:mm:ss").format(Calendar.getInstance().getTime() ));    System.out.println("This represents a skew of  "  + (Calendar.getInstance().getTimeInMillis()    rs.getServerTime().getTimeInMillis() )/1000 + " seconds from netsuite    (where positive time means the client clock is comparatively fast)."); }` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
