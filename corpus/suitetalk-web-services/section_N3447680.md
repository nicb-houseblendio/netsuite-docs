---
id: "section_N3447680"
type: "section"
title: "Session Management for SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Security > Session Management for SOAP Web Services"
parent: "chapter_N3445516"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3447680.html"
anchors: ["bridgehead_N3447809", "bridgehead_N3447864", "bridgehead_1508932737", "bridgehead_1508932980", "bridgehead_N3447901", "bridgehead_3819268808", "bridgehead_N3447951", "bridgehead_3705125415"]
sha256: "b370dd51e74e0c0531764e4aa0e587ead5303dbf60279ac3e5860c914335dfff"
---

Warning:

As of the 2020.1 endpoint, the login and logout operations are no longer working. This is because as of the 2020.1 endpoint you must use token-based authentication to login, instead of the login operation. For more information, see [Token-based Authentication (TBA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4247329078.html). The operation is still working for earlier endpoints that are still supported. For more information about supported endpoints, see [Support for Existing WSDL Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418621.html).

As of the 2020.2 SOAP web services endpoint, authentication through request-level credentials is not supported. The [Passport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452954.html#bridgehead_N3453226) complex type is not supported. If you attempt to authenticate through request-level credentials in SOAP web services 2020.2 and later endpoints, the web services request is not processed, and an error message is returned.

User credentials are not preferred as an authentication method for SOAP web services. If you are currently using this method, you should transition to use token-based authentication instead.

In NetSuite, session management includes:

-   [Session Timeouts](#bridgehead_N3447809)
    
-   [Session Limits](#bridgehead_N3447864)
    
-   [Manually Managing Cookies](#bridgehead_N3447901)
    

## Session Timeouts {#bridgehead_N3447809}

The Open Web Application Security Project (OWASP) provides the following guideline: All sessions should implement an absolute timeout, regardless of session activity. This timeout defines the maximum amount of time a session can be active. The session is closed and invalidated upon the defined absolute period. After the session is invalidated, the user must authenticate (log in) again in the web application and establish a new session. The absolute session timeout limits the amount of time possible for a potential attacker to use a hijacked session to impersonate a user.

Important:

To enhance the security of your account, and to comply with the OWASP guideline, there is an absolute session timeout implemented for SOAP web services sessions. Currently, the absolute session timeout value is set to 60 minutes, even if the session is active.

If you use sessions with your SOAP web services integrations, you must ensure that your SOAP web services calls are able to handle session timeouts. Your integrations should use sessionless protocols based on request-level credentials, such as user credentials or token-based authentication (TBA). Using TBA is preferred. See [Authentication for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3445710.html) for more information.

SOAP web services sessions automatically time out after 20 minutes of inactivity, requiring a login to resume activity. If the server resubmits the cookie during the first 20 minutes, the inactivity timer is reset.

If a SOAP web services operation takes more than 15 minutes to complete, it automatically times out. In this case, consider using asynchronous request processing. For more information, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

If you explicitly log out of a session, and then attempt to use the same session, a SESSION\_TIMED\_OUT error message is returned. Your code should be prepared to handle session timeouts by retrying if an InvalidSessionFault (SESSION\_TIMED\_OUT) error is received.

Important:

Do not make any integration decisions based on the value of the absolute timeout value or the idle session timeout values, as these values can be changed at any time without notice.

## Session Limits {#bridgehead_N3447864}

Session limits involve both user limits and account limits.

## User Limits {#bridgehead_1508932737}

A specific login (user name, account and password) that is used for a UI session can be used to create one or more sessions through SOAP web services by using the login operation. More SOAP web services sessions can occur concurrently, but the number of operations processed concurrently is limited. The UI session does not affect the SOAP web services sessions and operations.

Without a SuiteCloud Plus license, one user should create only one SOAP web services session using the login operation, and send requests using this session in one thread sequentially.

If the NetSuite server receives two login or other operations from the same user at the same moment, the second operation is rejected, and the error "Only one request may be made against a session at a time' is sent. The error indicates that the per user governance limit is exceeded.

Using the same login from multiple client applications, or multiple instances of the same application is NOT supported.

If you have a SuiteCloud Plus license, you can designate users as concurrent SOAP web services users. One SuiteCloud Plus license allows you to designate one user as concurrent SOAP web services user. One concurrent SOAP web services user can send up to 10 concurrent SOAP web services requests.

Note:

If the total account limit for concurrent requests is exceeded, one concurrent SOAP web services user might not be able to send 10 concurrent requests.

## Account Limits {#bridgehead_1508932980}

Note that starting from version 2017.2, web services concurrency is not only governed separately per user and authentication method, but also per account. For information about account concurrency limits, see [Web Services and RESTlet Concurrency Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1500275531.html).

Each SuiteCloud Plus license increases the account concurrency governance limit by 10, meaning that you can have 10 additional parallel requests at the same per account. The account base limit depends on your service tier. For details, see [Enabling Web Services Concurrent Users with SuiteCloud Plus](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3448861.html).

## Manually Managing Cookies {#bridgehead_N3447901}

When submitting SOAP web services requests, the NetSuite server can accept any SOAP document if it is valid against the NetSuite WSDL, and it does not matter how the SOAP document was generated. You must ensure that all cookies received from the server are managed and passed back to the server in subsequent calls. There are a total of three cookies that are initially returned in the HTTP header of the login response, including the JSESSIONID.

Note:

The JSESSIONID cookie is only generated if you use the Login or the [ssoLogin](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3526370.html) operation for authentication. If you use request-level credentials, this cookie is not generated.

Ensure that your client persists any cookies that our server sends you (re-submits the cookie on the next request). In Axis, this is accomplished by enabling **MaintainSession** on the generated Binding object. In .NET, this involves allocating a CookieContainer. If persistence is not maintained, you will receive the following error message: SESSION\_TIMED\_OUT - 'Your connection has timed out. Please log in again.'

## Example {#bridgehead_3819268808}

The following code shows the cookie information returned in the login response. The cookie information is contained in the Set-Cookie lines of the code.

          `HTTP/1.1 200 OK Date: Mon, 16 Oct 2017 13:34:48 GMT Content-Type: text/xml; charset=utf-8 X-N-OperationId: a8f84e6e-6300-4f92-9a1a-30fae3da1978 X-Netsuite-Approute: host=test.eng.netsuite.com;enter=2017-10-16 06:34:48.716;buf=785;versrc=passport;apco=err_cxn;ver=2018.1.0;dcid=000;exit=2017-10-16 06:34:48.720;events=setcookie,rule Set-Cookie: JSESSIONID=iR8lZOFn88GFV23ZVnnS0BUTi6V2fJZZzil02Xf9gyXvNTVNarxfIWRanvswN0LDYW-gKsBUo75gVslo42EfwTm-qlKnTDo5SynW_nc-Yvh0dQJVTzHokW9qGvoyn0jW!-477725890; path=/; HttpOnly Set-Cookie: NS_ROUTING_VERSION=LAGGING; path=/ Set-Cookie: NS_VER=2017.2.0; domain=test.eng.netsuite.com; path=/ P3P: CP="CAO PSAa OUR BUS PUR" Vary: User-Agent Connection: close` 
        

For each subsequent request, all of the cookies must be returned in the HTTP header to maintain the session as follows:

## C# {#bridgehead_N3447951}

          `NetSuiteService nss = new NetSuiteService(); nss.Url = https://webservices.netsuite.com/services/NetSuitePort_2017_1_0 ;  nss.CookieContainer = new CookieContainer();` 
        

Note:

This snippet assumes that your integration includes a `Using System.Net;` statement.

## Java with Axis 1.4 {#bridgehead_3705125415}

          `NetSuiteServiceLocator service = new DataCenterAwareNetSuiteServiceLocator(_properties.getProperty("login.acct")); service.setMaintainSession(true);` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Security](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3445516.html)
-   [Authentication for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3445710.html)
-   [Authorization for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3447510.html)
-   [Encryption for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3448169.html)
-   [Custom Field Security](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3448524.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
