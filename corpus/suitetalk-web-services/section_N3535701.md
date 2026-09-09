---
id: "section_N3535701"
type: "section"
title: "Creating and Submitting Records Using the PHP Toolkit"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services PHP Toolkit > Creating and Submitting Records Using the PHP Toolkit"
parent: "chapter_N3533866"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535701.html"
anchors: ["bridgehead_N3535761", "bridgehead_N3535785", "bridgehead_N3535822"]
sha256: "5f576d8032cfb0e3ea26b61ae2d658b5797d0a3ba9a6d4312013cacff8d8f97f"
---

These sections provide basic examples for creating and submitting NetSuite records using the PHP toolkit.

-   [Creating a Record with PHP](#bridgehead_N3535761)
    
-   [Creating a Record with the setFields Method](#bridgehead_N3535785)
    
-   [Submitting a Record](#bridgehead_N3535822)
    

## Creating a Record with PHP {#bridgehead_N3535761}

The following example shows how to create and submit a Purchase Order. In this case, the Purchase Order object is created then populated one field at a time.

Note that after the Purchase Order is instantiated, the IDE should automatically start suggesting members of the PurchaseOrder object using its code completion mechanism.

          `// Include the PHP Toolkit Library require_once '../PHPToolkit/NetSuiteService.php';   // Instantiate a service $service = new NetSuiteService();   // Create Purchase Order object $po = new PurchaseOrder();    // Create entity record $po->entity = new RecordRef();   // PO internal ID = 38 $po->entity->internalId = 38;   // Create PO Item sublist $po->itemList = new PurchaseOrderItemList();    // Create PO Item $poi = new PurchaseOrderItem();  $poi->item = new RecordRef();    // Set Item details $poi->item->internalId = 15;  $poi->quantity = 5;    // Attach items array to PO $po->itemList->item = array($poi);` 
        

## Creating a Record with the setFields Method {#bridgehead_N3535785}

An alternative method to create the object is to use array notation to set the object fields. The advantage is more compact code; the disadvantage is that code completion will not work.

The following example creates the same Purchase Order object using the setFields method:

          `// Create the Purchase Order object  $po = new PurchaseOrder();    // Create array of fields  $purchaseOrderFields = array('entity' => array('internalId' => 38), 'itemList' => array('item' => array( array('item' => array('internalId' => 15), 'quantity' => 5)) ) );    // Call setFields to recursively create objects and populate their fields  setFields($po, $purchaseOrderFields);` 
        

In addition to creating and populating objects, the setFields method performs basic type and field checking to make sure the array structure corresponds to the expected object hierarchy and types.

Note:

The setFields method is defined in the NSPHPClient.php helper file, which is included automatically by NetSuiteService.php

## Submitting a Record {#bridgehead_N3535822}

After the object is created and populated, the object can be submitted to NetSuite in one of the operations supported by the type of object you have created. The following code sample shows the **add** operation:

          `// Create Add request $request = new AddRequest();    // Attach the Purchase Order to the request $request->record = $po;    // Submit the record and save the response $addResponse = $service->add($request);` 
        

The **add** operation returns a ReadResponse object that is used to access the result of the operation. The following code sample reads and displays a simple textual indication of the result:

          `if (!$addResponse->writeResponse->status->isSuccess)  {     echo "ADD ERROR";  }  else  {     echo "ADD SUCCESS, id " . $addResponse->writeResponse->baseRef->internalId;  }` 
        

Note:

The PHP Toolkit package contains more code examples in the Samples folder.

### Related Topics

-   [PHP Toolkit Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534011.html)
-   [Downloading the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534718.html)
-   [Configuring an Environment for the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3534858.html)
-   [Creating a SOAP Web Services PHP Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535140.html)
-   [Logging SOAP Requests and Responses Using the PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535863.html)
-   [Troubleshooting PHP and SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3535978.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
