---
id: "section_N3534011"
type: "section"
title: "PHP Toolkit Overview"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services PHP Toolkit > PHP Toolkit Overview"
parent: "chapter_N3533866"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534011.html"
anchors: ["bridgehead_N3534048"]
sha256: "65ad0a222d7475f21a82e5816efdaf79774c78db687cbf749e3245e5b22a9e57"
---

Important:

Using PHP scripts with SOAP web services requires PHP version 5.6 or later.

NetSuite provides a library and tools to assist in the development of PHP applications that interface to the SOAP web services platform.

The NetSuite PHP toolkit for SOAP web services is a core library containing all classes, objects and methods parsed from the WSDL of a SOAP web services endpoint. The toolkit also comes with several helper functions that can be used to simplify working with arrays and objects.

Important:

Each PHP Toolkit is specific to a SOAP web services endpoint. You must download the correct version of the toolkit for the endpoint you are using. Also, updating to a new endpoint requires an update of the toolkit. **To use the 2025.2 PHP Toolkit, you must upgrade to the 2025.2 WSDL. The 20241 PHP Toolkit does not officially support different WSDL versions.**

## Updating Existing PHP Code {#bridgehead_N3534048}

NetSuite offered a completely revamped PHP Toolkit as part of 2012.2. As of 2012.2, the PHP Toolkit has the ability to generate proxy classes for every new NetSuite WSDL, creating a development environment similar to Axis or .NET.

Additionally, the new toolkit uses a different programming model (the use of proxy classes over pure associative arrays, though the latter is still supported).

If you upgrade to any version of the PHP Toolkit later than 2012.2, existing PHP applications created using previous versions of the toolkit will need to be updated. To understand the nature of the coding changes, see the table below. Also see the sample applications that come with the new toolkit.

|  | PHP Toolkit 2012.2 and Later | PHP Toolkit Versions Older than 2012.2 |
| --- | --- | --- |
| Record object initialization | Each record type can now be initialized using the same record type name. Example - To initialize a Customer record object: $CustomerRec = new Customer(); | Initialize the object using the object nsComplexObject. Example - To initialize a Customer record object: $CustomerRec = new nsComplexObject('Customer'); |
| Object type Initialization All object types are listed and explained in [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html). | Each complex, search and custom field type is initialized using the same object type name: Example - To initialize a basic search for customers: $selectTypeField = new RecordRef(); To initialize a recordRef object: $selectTypeField = new RecordRef(); | These objects are initialized using the object nsComplexObject. Example - To initialize a basic search for customers: $search = new nsComplexObject('CustomerSearchBasic'); To initialize a recordRef object: $selectTypeField = new nsComplexObject ('RecordRef'); |
| Calling the NetSuite SOAP web services operations | The operations are called from the **service** object instantiated from the NetSuiteService class (NetSuiteService.php). Example - $service = new NetSuiteService(); … $addResponse = $service->add($request); | The operations are called from the **client** object instantiated from the nsClient class (declared on the phptoolkit.php). Example - $myNSclient = new nsClient( nsHost::live ); … $addResponse = $myNSclient->add($contact); |
| Request object | You must instantiate a request object depending on the kind of operation. This request object will accept the Record object, which will then be set to the operation. Each operation has a corresponding request type.
-   AddRequest for add operation
-   AddListRequest for addList operation
-   SearchRequest for search operation.

Example - To add a customer:

$service = new NetSuiteService();

$CustomerRec = new Customer();

…

$request = new AddRequest();

$request->record = $CustomerRec;

… $addResponse = $service->add($request); | None. The record object is directly set to the operation. Example - To add a customer: $CustomerRec = new nsComplexObject('Customer'); … $addResponse = $myNSclient->add($CustomerRec); |
| The setFields method | A function to set an array of field objects to the record object. Example - $customerRec = new Customer(); $customerFields = array (

'isPerson' => true,

'firstName' => $firstName,

'lastName' => $lastName,

'companyName' => $companyName

); setFields($customerRec, $ customerFields); | This is a method of the record object used to set the array of field values to the record. Example - $customerFields = array (

'isPerson' => true,

'firstName' => $firstName,

'lastName' => $lastName,

'companyName' => $companyName

);

// create Customer record

$customer = new nsComplexObject('Customer');

// set fields

$customer-\>setFields($customerFields);



 |

### Related Topics

-   [Downloading the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534718.html)
-   [Configuring an Environment for the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534858.html)
-   [Creating a SOAP Web Services PHP Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535140.html)
-   [Creating and Submitting Records Using the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535701.html)
-   [Logging SOAP Requests and Responses Using the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535863.html)
-   [Troubleshooting PHP and SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535978.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
