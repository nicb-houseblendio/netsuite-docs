---
id: "section_N3687718"
type: "section"
title: "Purchase Order"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Purchase Order"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3687718.html"
anchors: ["bridgehead_N3687756", "bridgehead_N3688131", "bridgehead_N3688168", "bridgehead_N3688177", "procedure_N3688189", "bridgehead_N3688200", "bridgehead_N3688254", "bridgehead_N3688268", "bridgehead_N3688298", "bridgehead_3820143024", "bridgehead_N28481871", "bridgehead_N28481961", "bridgehead_N28482041", "bridgehead_N28482101"]
sha256: "6d880000a441a4c94c3ff898163594d9348c88a84cd9590b1fb183a107091df4"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161165602348.html).

A purchase order transaction authorizes the purchase of goods, services, or both. This transaction tracks items expected to be received, items received, and items yet to be received. A purchase order has no accounting impact until the included items are received. This transaction is enabled when the Purchase Orders feature is enabled.

For more details about this type of transaction, see [Purchasing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2399286.html).

The purchase order record is defined in the [tranPurch (purchases)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/purchases.xsd) XSD.

## Supported Operations {#bridgehead_N3687756}

The following operations can be used with purchase order records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3688131}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [purchase order](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/purchaseorder.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Note:

The balance field is only returned when using advanced search. It is not returned when using the <Record>SearchBasic search object. In advanced search, you must set the bodyFieldsOnly preference to false. The balance field is not returned if the bodyFieldsOnly preference is set to true. For more information, see [bodyFieldsOnly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html#bridgehead_N3423730).

## Usage Notes {#bridgehead_N3688168}

## Working with Purchase Order Sublists {#bridgehead_N3688177}

The SOAP Schema Browser includes all sublists associated with the purchase order record. See the following information for usage notes regarding specific purchase order sublists. Usage notes are not provided for every list type.

## PurchaseOrderApprovalsList {#procedure_N3688189}

This is a read-only list available on an update and maps to the History/Approvals subtab in the UI.

## Accessing Serial or Lot Number Data for Line Items {#bridgehead_N3688200}

Code to access serial number or lot number data varies according to whether the Advanced Bin Management / Numbered Inventory Management feature is enabled.

For more details, see [Updating SOAP Web Services Code When Advanced Bin / Numbered Inventory Management is Enabled](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3745415.html).

## Linking Purchase Orders to a Vendor Bill {#bridgehead_N3688254}

SOAP web services endpoints support transaction links between purchase orders and vendor bills, allowing you to populate a vendor bill with the items and expenses from one or more purchase orders. Two approaches are supported for linking purchase order(s) to a vendor bill.

Important:

When you initialize a vendor bill from a purchase order, the purchase order gets transformed but any attached files are not transferred to the vendor bill. You can apply a workaround consisting of (aftersubmit) user event script on the vendor bill, that checks every source transaction for the new vendor bill and attaches their media files to it.

Also, when you initialize a vendor bill, there are two possibilities for the value of the account field on the vendor bill.

-   If you **have not** populated the Default Payables Account field under the Financial subtab in the Vendor record, SOAP web services populate the Account field of the initialized vendor bill with the account most recently used on a vendor bill.
    
-   If you **have** populated the Default Payables Account field under the Financial subtab in the Vendor record, SOAP web services populate the Account field of the initialized vendor bill with the same field value.
    

## First Approach {#bridgehead_N3688268}

The simpler approach is to use the purchaseOrderList in a vendor bill add request. When you include purchase order internalId or externalId value(s) in the purchaseOrderList, all of the items and expenses from the specified purchase order(s) are added to the vendor bill's itemList and expenseList. Use this approach when you want a vendor bill to contain all of the line items from linked purchase orders. See [SOAP Request (Sample 1 - Approach 1)](#bridgehead_N28481871) for details.

Important:

If you set values for a vendor bill's purchaseOrderList in a request, you cannot set values for its itemList or expenseList in the same request.

## Second Approach {#bridgehead_N3688298}

The second approach is to send a vendor bill initialize request that references one or more purchase orders by id. The initializeResponse returns itemList and expenseList data from the referenced purchase order(s). This data includes orderDoc and orderLine field values that together provide a unique identifier for each line item. You can then send a vendor bill add request setting values for the vendor bill's itemList and expenseList with data copied from the response. You should copy only the data from the specific purchase order items and expenses that you want to be included in the vendor bill. This approach lets you select a subset of line items from each linked purchase order, rather than including all linked purchase order line items in a vendor bill.

In the second approach, you will use the initialize operation, which supports multiple purchase orders per vendor. Also, the orderDoc and orderLine fields are included in the vendor bill itemList and expenseList. For details, see [SOAP Request (Sample 2 - Approach 2)](#bridgehead_N28481961) and the accompanying SOAP Response and Java.

Important:

If you reference multiple purchase orders with either of these approaches, all referenced purchase orders must be for the same vendor.

## Code Samples {#bridgehead_3820143024}

## SOAP Request (Sample 1 - Approach 1) {#bridgehead_N28481871}

Using an add request to populate a vendor bill with the items and expenses from multiple purchase orders:

          `<soapenv:Body>            <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <record xsi:type="ns6:VendorBill" xmlns:ns6="urn:purchases_2017_1.transactions.webservices.netsuite.com">                    <ns6:entity internalId="98" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns6:purchaseOrderList xsi:type="ns8:RecordRefList" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com">                        <ns8:recordRef internalId="2659" type="purchaseOrder" xsi:type="ns8:RecordRef"/>                        <ns8:recordRef internalId="2661" type="purchaseOrder" xsi:type="ns8:RecordRef"/>                    </ns6:purchaseOrderList>                </record>            </add>        </soapenv:Body>` 
        

## SOAP Request (Sample 2 - Approach 2) {#bridgehead_N28481961}

Using an initialize request to populate a vendor bill with the items and expenses from multiple purchase orders. This approach lets you select a subset of line items from each linked purchase order, rather than including all linked purchase order line items in a vendor bill.

          `<soapenv:Body>            <initialize xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <initializeRecord>                    <ns7:type xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com">vendorBill</ns7:type>                    <ns8:referenceList xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com">                        <ns8:initializeRef internalId="2659" type="purchaseOrder"/>                        <ns8:initializeRef internalId="2661" type="purchaseOrder"/>                    </ns8:referenceList>                </initializeRecord>            </initialize>        </soapenv:Body>` 
        

## SOAP Response (Sample 2) {#bridgehead_N28482041}

          `<initializeResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <readResponse>                <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                <record xsi:type="tranPurch:VendorBill" xmlns:tranPurch="urn:purchases_2017_1.transactions.webservices.netsuite.com">                   <tranPurch:entity internalId="98" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                      <platformCore:name>Test Vendor</platformCore:name>                   </tranPurch:entity>                   <tranPurch:subsidiary internalId="1" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                      <platformCore:name>Parent Company</platformCore:name>                   </tranPurch:subsidiary>                   <tranPurch:approvalStatus internalId="2" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                      <platformCore:name>Approved</platformCore:name>                   </tranPurch:approvalStatus>                   <tranPurch:postingPeriod internalId="126" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                      <platformCore:name>Apr 2012</platformCore:name>                   </tranPurch:postingPeriod>                   <tranPurch:tranDate>2012-04-30T00:00:00.000-07:00</tranPurch:tranDate>                   <tranPurch:currencyName>US USD</tranPurch:currencyName>                   <tranPurch:exchangeRate>1.0</tranPurch:exchangeRate>                   <tranPurch:dueDate>2012-04-30T00:00:00.000-07:00</tranPurch:dueDate>                   <tranPurch:userTotal>121.0</tranPurch:userTotal>                   <tranPurch:currency internalId="1" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                      <platformCore:name>US USD</platformCore:name>                   </tranPurch:currency>                   <tranPurch:expenseList>                      <tranPurch:expense>                         <tranPurch:orderDoc>2661</tranPurch:orderDoc>                         <tranPurch:orderLine>1</tranPurch:orderLine>                         <tranPurch:category internalId="2" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                            <platformCore:name>Entertainment</platformCore:name>                         </tranPurch:category>                         <tranPurch:account internalId="59" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                            <platformCore:name>Advertising</platformCore:name>                         </tranPurch:account>                         <tranPurch:amount>2.0</tranPurch:amount>                         <tranPurch:isBillable>false</tranPurch:isBillable>                      </tranPurch:expense>                      <tranPurch:expense>                         <tranPurch:orderDoc>2659</tranPurch:orderDoc>                         <tranPurch:orderLine>1</tranPurch:orderLine>                         <tranPurch:category internalId="2" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                            <platformCore:name>Entertainment</platformCore:name>                         </tranPurch:category>                         <tranPurch:account internalId="59" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                            <platformCore:name>Advertising</platformCore:name>                         </tranPurch:account>                         <tranPurch:amount>5.0</tranPurch:amount>                         <tranPurch:isBillable>false</tranPurch:isBillable>                      </tranPurch:expense>                      <tranPurch:expense>                         <tranPurch:orderDoc>2661</tranPurch:orderDoc>                         <tranPurch:orderLine>2</tranPurch:orderLine>                         <tranPurch:category internalId="1" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                            <platformCore:name>Travel</platformCore:name>                         </tranPurch:category>                         <tranPurch:account internalId="59" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                            <platformCore:name>Advertising</platformCore:name>                         </tranPurch:account>                         <tranPurch:amount>10.0</tranPurch:amount>                         <tranPurch:isBillable>false</tranPurch:isBillable>                      </tranPurch:expense>                      <tranPurch:expense>                         <tranPurch:orderDoc>2659</tranPurch:orderDoc>                         <tranPurch:orderLine>2</tranPurch:orderLine>                         <tranPurch:category internalId="1" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                            <platformCore:name>Travel</platformCore:name>                         </tranPurch:category>                         <tranPurch:account internalId="59" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                            <platformCore:name>Advertising</platformCore:name>                         </tranPurch:account>                         <tranPurch:amount>100.0</tranPurch:amount>                         <tranPurch:isBillable>false</tranPurch:isBillable>                      </tranPurch:expense>                   </tranPurch:expenseList>                   <tranPurch:itemList>                      <tranPurch:item>                         <tranPurch:item internalId="39" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                            <platformCore:name>Item No Tax 2 Lbs(All)</platformCore:name>                         </tranPurch:item>                         <tranPurch:orderDoc>2659</tranPurch:orderDoc>                         <tranPurch:orderLine>3</tranPurch:orderLine>                         <tranPurch:quantity>1.0</tranPurch:quantity>                         <tranPurch:description>Item No Tax 2 Lbs(All)</tranPurch:description>                         <tranPurch:rate>1.00</tranPurch:rate>                         <tranPurch:amount>1.0</tranPurch:amount>                         <tranPurch:isBillable>false</tranPurch:isBillable>                      </tranPurch:item>                      <tranPurch:item>                         <tranPurch:item internalId="38" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                            <platformCore:name>Item No Tax 2 Lbs(US)</platformCore:name>                         </tranPurch:item>                         <tranPurch:orderDoc>2659</tranPurch:orderDoc>                         <tranPurch:orderLine>4</tranPurch:orderLine>                         <tranPurch:quantity>1.0</tranPurch:quantity>                         <tranPurch:rate>1.00</tranPurch:rate>                         <tranPurch:amount>1.0</tranPurch:amount>                         <tranPurch:isBillable>false</tranPurch:isBillable>                      </tranPurch:item>                      <tranPurch:item>                         <tranPurch:item internalId="36" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                            <platformCore:name>Item Tax 2 Lbs(All)</platformCore:name>                         </tranPurch:item>                         <tranPurch:orderDoc>2661</tranPurch:orderDoc>                         <tranPurch:orderLine>3</tranPurch:orderLine>                         <tranPurch:quantity>1.0</tranPurch:quantity>                         <tranPurch:rate>1.00</tranPurch:rate>                         <tranPurch:amount>1.0</tranPurch:amount>                         <tranPurch:isBillable>false</tranPurch:isBillable>                      </tranPurch:item>                      <tranPurch:item>                         <tranPurch:item internalId="29" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                            <platformCore:name>Item Tax 2 Lbs(US)</platformCore:name>                         </tranPurch:item>                         <tranPurch:orderDoc>2661</tranPurch:orderDoc>                         <tranPurch:orderLine>4</tranPurch:orderLine>                         <tranPurch:quantity>1.0</tranPurch:quantity>                         <tranPurch:rate>1.00</tranPurch:rate>                         <tranPurch:amount>1.0</tranPurch:amount>                         <tranPurch:isBillable>false</tranPurch:isBillable>                      </tranPurch:item>                   </tranPurch:itemList>                   <tranPurch:customFieldList xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                      <platformCore:customField internalId="custbody_633637_asubmit" xsi:type="platformCore:BooleanCustomFieldRef">                         <platformCore:value>false</platformCore:value>                      </platformCore:customField>                      <platformCore:customField internalId="custbody_633637_bsubmit" xsi:type="platformCore:BooleanCustomFieldRef">                         <platformCore:value>false</platformCore:value>                      </platformCore:customField>                      <platformCore:customField internalId="custbody_633637_bload" xsi:type="platformCore:BooleanCustomFieldRef">                         <platformCore:value>false</platformCore:value>                      </platformCore:customField>                   </tranPurch:customFieldList>                </record>             </readResponse>          </initializeResponse>` 
        

## Java (Sample 2) {#bridgehead_N28482101}

          `public void initializeVendorBillByPurchaseOrders() throws Exception    {       this.login();         InitializeRefList purchaseOrderList = new InitializeRefList();       InitializeRef[] initializeRefArray = new InitializeRef[2];       initializeRefArray[0] = new InitializeRef(null, InitializeRefType.purchaseOrder, "510", null);       initializeRefArray[1] = new InitializeRef(null, InitializeRefType.purchaseOrder, "511", null);       purchaseOrderList.setInitializeRef(initializeRefArray);       InitializeRecord initializeRecord = new InitializeRecord(InitializeType.vendorBill, null, null, purchaseOrderList);       ReadResponse response = _port.initialize(initializeRecord);       VendorBill vendorBill = (VendorBill) response.getRecord();    }` 
        

### Related Topics

-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Usage Notes for Transaction Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3658677.html)
-   [Transaction Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659492.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
