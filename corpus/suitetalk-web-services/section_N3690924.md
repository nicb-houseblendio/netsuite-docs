---
id: "section_N3690924"
type: "section"
title: "Sales Order"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Sales Order"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3690924.html"
anchors: ["bridgehead_N3690960", "bridgehead_N3691229", "bridgehead_N3691266", "bridgehead_3946198374", "bridgehead_N3691275", "bridgehead_N3691318", "bridgehead_N3691330", "bridgehead_N3691374", "bridgehead_N3691390", "bridgehead_N28489331", "bridgehead_N28489391", "bridgehead_N3691420", "bridgehead_N28489541", "bridgehead_N28489601", "bridgehead_N28489661", "bridgehead_N3691464", "procedure_N3691476", "bridgehead_N3691487", "bridgehead_N3691511", "bridgehead_N3691523", "bridgehead_N3691545", "bridgehead_N3691598", "bridgehead_N3691664"]
sha256: "92544fad7915ba13f3d3455552bd6464645097cc6a131cdb616f738a6885aafd"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159665260887.html).

A sales order transaction records a commitment to sell goods or services to a customer. Sales orders have no accounting impact until items are shipped or services are completed.

For details about this type of transaction, see [Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1215966.html).

The sales order record is defined in the [tranSales (sales)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/sales.xsd) XSD.

## Supported Operations {#bridgehead_N3690960}

The following operations can be used to modify sales order records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3691229}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [sales order](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/salesorder.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Note:

The balance field is only returned when using advanced search. It is not returned when using the <Record>SearchBasic search object. In advanced search, you must set the bodyFieldsOnly preference to false. The balance field is not returned if the bodyFieldsOnly preference is set to true. For more information, see [bodyFieldsOnly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html#bridgehead_N3423730).

## Usage Notes {#bridgehead_N3691266}

## Working with Credit Card Data {#bridgehead_3946198374}

When working with credit card data, be aware of the following security features:

-   When adding a transaction that uses a credit card number, you cannot identify the credit card number using a masked value such as \*\*\*\*\*\*\*\*\*\*\*\*5151. You must enter the full 16-digit number, or you can identify an existing credit card record through a RecordRef. (You can identify the full number using the **ccNumber** field. You can reference an existing record using the **creditCard** field.)
    
-   Searches do not work if they include the operator **is** or **isNot** in conjunction with the ccNumber field. The only search operators that can apply to this field are **empty** and **notEmpty**.
    

## Initializing Sales Orders {#bridgehead_N3691275}

You can initialize a sales order from an [Estimate/Quote](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3673214.html) or an [Opportunity](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3684743.html).

The SOAP web services initialize operation emulates the UI workflow by prepopulating fields on transaction line items with values from a related record. For more information about this operation, see [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html).

## Setting Handling Cost {#bridgehead_N3691318}

If you want to set a value for handlingCost, be aware of the following guidelines.

## Only Certain Shipping Methods Allow Handling Cost To Be Set {#bridgehead_N3691330}

In both the UI and in SOAP web services, the default behavior of the system is that you cannot specify a handling cost on a new sales order. To be able to enter a value for handling cost, you must choose a shipping method that enables the handling cost field.

You can identify an appropriate shipping method by reviewing the details for the corresponding shipping item. Go to Lists > Accounting > Shipping Items, then select the shipping item you want to review (each shipping item corresponds with a shipping method). In the item record, review the details on the Handling Rate subtab. If the Handling - No Handling Charge is **not** selected, then choosing this shipping item lets you set a handlingCost value.

During an add operation, you must set the shipMethod value in the same SOAP request where you set the handlingCost value. If you fail to set any value for shipMethod, or if you choose a value that does not enable the handling cost field, the system generates an error reading in part 'You do not have permissions to set a value for element handlingcost.'

## You Must Specify a Shipping Cost {#bridgehead_N3691374}

If you are doing an add operation, be aware that in some cases the system may overwrite the handlingCost value specified in your SOAP request. To avoid this, make sure that your SOAP request include a shippingCost value. If you fail to include a shippingCost, the system overwrites your handlingCost value with an automatically generated value.

This behavior is specific to the add operation. During an update, it is possible to set a value for handlingCost without specifying the shippingCost.

## Adding a Sales Order with an Item Sublist {#bridgehead_N3691390}

## C# {#bridgehead_N28489331}

          `public virtual void  addSalesOrder()       {          // This operation requires a valid session          this.login(true);                    SalesOrder so = new SalesOrder();          // Set customer entity                    _out.writeLn("\nPlease enter the following customer information. "           + "Note that some fields have already been populated. ");          _out.write("  Customer entity name: ");                    CustomerSearch custSearch = new CustomerSearch();          SearchStringField customerEntityID = new SearchStringField();          customerEntityID.@operator = SearchStringFieldOperator.@is;          customerEntityID.operatorSpecified = true;          customerEntityID.searchValue = _out.readLn();                    CustomerSearchBasic custBasic = new CustomerSearchBasic();          custBasic.entityId = customerEntityID;                    //custSearch.setEntityId(customerEntityID);                    custSearch.basic = custBasic;                    // Search for the customer entity          SearchResult res = _service.search(custSearch);                    if (res.status.isSuccess)          {             if (res.recordList != null && res.recordList.Length == 1)             {                RecordRef customer = new RecordRef();                customer.type = RecordType.customer;                customer.typeSpecified = true;                System.String entID = ((Customer) (res.recordList[0])).entityId;                customer.name = entID;                customer.internalId = ((Customer) (res.recordList[0])).internalId;                so.entity = customer;                                // set the transaction date and status                so.tranDate = new System.DateTime();                so.orderStatus = SalesOrderOrderStatus._pendingApproval;                                // Enter the nsKey for inventory items to be added to the SO                _out.writeLn("\nPlease enter the nsKey values for                 INVENTORY ITEMS separated by                commas (do not enter discount or subtotal items).");                System.String itemKeys = _out.readLn();                System.String[] itemKeysArray = itemKeys.Split(new Char[] {','});                                ReadResponse[] readRes = getInventoryItemList(itemKeysArray);                                // Determine the number of valid inventory item nsKeys entered                ArrayList vec = new ArrayList();                for (int a = 0; a < readRes.Length; a++)                {                   if (readRes[a].record != null)                   {                      vec.Add(readRes[a].record);                   }                }                SalesOrderItem[] salesOrderItemArray = new SalesOrderItem[vec.Count];                                // Create the correct sales order items and populate the                // quantity                for (int i = 0; i < vec.Count; i++)                {                   if (vec[i] is InventoryItem)                   {                      RecordRef item = new RecordRef();                      item.type = RecordType.inventoryItem;                      item.typeSpecified = true;                      item.internalId = ((InventoryItem) (vec[i])).internalId;                      salesOrderItemArray[i] = new SalesOrderItem();                      salesOrderItemArray[i].item = item;                                            _out.writeLn("\nPlease enter quantity for " + ((InventoryItem)                      (vec[i])).itemId);                      System.Double quantity = System.Double.Parse(_out.readLn());                      salesOrderItemArray[i].quantity = quantity;                      salesOrderItemArray[i].quantitySpecified = true;                   }                }                                   //SalesOrderItemList salesOrderItemList = new                   SalesOrderItemList(salesOrderItemArray, true);                //TODO: No constructor present for two argument.                SalesOrderItemList salesOrderItemList = new SalesOrderItemList();                salesOrderItemList.item = salesOrderItemArray;                 so.itemList = salesOrderItemList;                                WriteResponse writeRes = _service.add(so);                if (writeRes.status.isSuccess)                {                   _out.writeLn("\nSales order created successfully");                }                else                {                   _out.error(getStatusDetails(writeRes.status));                }             }             else             {                _out.writeLn("\nSales order is not created because 0 or more than 1                   customer records found for the entityID given");             }          }          else          {             _out.error(getStatusDetails(res.status));          }       }` 
        

## Java {#bridgehead_N28489391}

          `public void addSalesOrder() throws RemoteException,          ExceededUsageLimitFault, UnexpectedErrorFault, InvalidSessionFault,          ExceededRecordCountFault {       // This operation requires a valid session       this.login(true);        SalesOrder so = new SalesOrder();       // Set customer entity        _console.writeLn("\nPlease enter the following customer information. "             + "Note that some fields have already been populated. ");       _console.write("  Customer entity name: ");        CustomerSearch custSearch = new CustomerSearch();       SearchStringField customerEntityID = new SearchStringField();       customerEntityID.setOperator(SearchStringFieldOperator.is);       customerEntityID.setSearchValue(_console.readLn());              CustomerSearchBasic custBasic = new CustomerSearchBasic();       custBasic.setEntityId(customerEntityID);              //custSearch.setEntityId(customerEntityID);        custSearch.setBasic(custBasic);              // Search for the customer entity       SearchResult res = _port.search(custSearch);        if (res.getStatus().isIsSuccess()) {          if (res.getRecordList().getRecord()!=null && res.getRecordList().getRecord().length == 1) {             RecordRef customer = new RecordRef();             customer.setType(RecordType.customer);             String entID = ((Customer) (res.getRecordList().getRecord(0)))                   .getEntityId();             customer.setName(entID);             customer.setInternalId(((Customer) (res.getRecordList()                   .getRecord(0))).getInternalId());             so.setEntity(customer);              // set the transaction date and status             so.setTranDate(Calendar.getInstance());             so.setOrderStatus(SalesOrderOrderStatus._pendingApproval);              // Enter the nsKey for inventory items to be added to the SO             _console                   .write("\nPlease enter the Internal Ids values for INVENTORY ITEMS separated             by commas (do not enter discount or subtotal items): ");             String itemKeys = _console.readLn();             String[] itemKeysArray = itemKeys.split(",");              ReadResponse[] readRes = getInventoryItemList(itemKeysArray);              // Determine the number of valid inventory item nsKeys entered             Vector vec = new Vector();             for (int a = 0; a < readRes.length; a++) {                if (readRes[a].getRecord() != null) {                   vec.add(readRes[a].getRecord());                }             }             SalesOrderItem[] salesOrderItemArray = new SalesOrderItem[vec                   .size()];              // Create the correct sales order items and populate the             // quantity             for (int i = 0; i < vec.size(); i++) {                if (vec.get(i) instanceof InventoryItem) {                   RecordRef item = new RecordRef();                   item.setType(RecordType.inventoryItem);                   item.setInternalId(((InventoryItem) (vec.get(i)))                         .getInternalId());                   salesOrderItemArray[i] = new SalesOrderItem();                   salesOrderItemArray[i].setItem(item);                    _console.write("\nPlease enter quantity for "                         + ((InventoryItem) (vec.get(i))).getItemId() + ": ");                   Double quantity = Double.valueOf(_console.readLn());                   salesOrderItemArray[i].setQuantity(quantity);                }             }             SalesOrderItemList salesOrderItemList = new SalesOrderItemList(                   salesOrderItemArray, true);             so.setItemList(salesOrderItemList);              WriteResponse writeRes = _port.add(so);             if (writeRes.getStatus().isIsSuccess()) {                _console.writeLn("\nSales order created successfully");             } else {                _console.error(getStatusDetails(writeRes.getStatus()));             }          } else {             _console                   .writeLn("\nSales order is not created because 0 or more than 1 customer                   records found for the entityID given");          }       } else {          _console.error(getStatusDetails(res.getStatus()));       }     }` 
        

## Setting the Shipping Address on a Sales Order {#bridgehead_N3691420}

The following code illustrates how to set the shipTo address on a sales order.

## SOAP Request {#bridgehead_N28489541}

          `<soapenv:Body> <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <record xsi:type="ns6:SalesOrder" xmlns:ns6="urn:sales_2017_1.transactions.webservices.netsuite.com">    <ns6:entity internalId="103 customer" xsi:type="ns7:RecordRef"        xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com">       <ns7:name xsi:type="xsd:string">Vintrust</ns7:name>    </ns6:entity>    <ns6:tranDate xsi:type="xsd:dateTime">2006-03-07T18:16:44.000Z</ns6:tranDate>    <ns6:orderStatus xsi:type="ns8:SalesOrderOrderStatus"        xmlns:ns8="urn:types.sales_2017_1.transactions.webservices.netsuite.com">_pendingApproval    </ns6:orderStatus>    <ns6:shipAddressList internalId="84" xsi:type="ns9:RecordRef"        xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com"/>    <ns6:itemList replaceAll="true" xsi:type="ns6:SalesOrderItemList">       <ns6:item xsi:type="ns6:SalesOrderItem">          <ns6:item internalId="18 inventoryItem" xsi:type="ns10:RecordRef"              xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com"/>          <ns6:quantity xsi:type="xsd:double">2.0</ns6:quantity>       </ns6:item>    </ns6:itemList> </record> </add> </soapenv:Body>` 
        

## C# {#bridgehead_N28489601}

          `Customer customer = // some customer CustomerAddressbook shipTo = // some customer address book entry RecordRef rr = new RecordRef(); rr.setInternalId(shipTo.getInternalId()); rr.setName("addressBook"); salesOrder.setShipAddressList(rr);` 
        

## Java {#bridgehead_N28489661}

          `//block setting shipping address to something other than default RecordRef altShipAddress = new RecordRef(); altShipAddress.setInternalId("84"); so.setShipAddressList(altShipAddress); //end block WriteResponse writeRes = _port.add(so);` 
        

## Working with Sales Order Sublists {#bridgehead_N3691464}

The SOAP Schema Browser includes all sublists associated with the sale order record. See the following information for usage notes regarding specific sales order sublists. Note that usage notes are not provided for every sublist type.

## SalesOrderSalesTeamList {#procedure_N3691476}

This list is only available when the Team Selling feature is enabled.

## Calculating Shipping Cost for Sales Orders {#bridgehead_N3691487}

SOAP web services calculation of shipping cost for sales orders varies slightly from the UI behavior. Because the sales order includes a Calculate Shipping button in the UI, updates to item quantity or other values that may impact shipping cost do not automatically recalculate that field's value in the UI. In SOAP web services, updates to item quantity or other values that impact shipping cost always result in recalculation of altshippingcost. If your account is set up to automatically charge for shipping, this defaults to the value that corresponds to the shipping method selected. To prevent this recalculation, resubmit the value for altshippingcost whenever you update item quantity or other fields that impact shipping cost.

Note that this SOAP web services behavior applies when the Multiple Shipping Routes feature is not enabled. For details about SOAP web services behavior with this feature enabled, see [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html).

## Sales Order Payment Terms and Payment Methods {#bridgehead_N3691511}

The NetSuite UI validates payment method values against payment terms values on sales order records, preventing values that do not match. In endpoints prior to 2010.1, SOAP web services allows the saving of both fields' values, even if they do not match. This behavior may result in unexpected errors on payments. You should not attempt to set payment method and terms at the same time for endpoints prior to 2010.1.

## Associating Sales Orders with Opportunities {#bridgehead_N3691523}

You can associate estimates, cash sales, sales orders, and invoices with opportunities. After a transaction other than an estimate is associated with an opportunity, the opportunity's status is automatically set to **Closed Won**. After an opportunity's status is set to **Closed Won**, it is no longer available to be selected on other cash sale, sales order, or invoice records.

## Accessing Serial or Lot Number Data for Line Items {#bridgehead_N3691545}

As of the 2011.2 endpoint, code to access serial number or lot number data varies according to whether the Advanced Bin Management / Numbered Inventory Management feature is enabled.

-   If this feature is enabled, you must use the 2011.2 endpoint or later to access the [Inventory Detail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3744760.html) subrecord and the most up-to-date bin and numbered inventory fields. You need to update any SOAP web services code from a previous endpoint that accesses these fields, to avoid errors or unexpected results.
    
-   If this feature is not enabled, you do not need to use the inventory detail record to access bin and numbered inventory fields and you do not need to update any related SOAP web services code from prior to 2011.2.
    

For more details, see [Updating SOAP Web Services Code When Advanced Bin / Numbered Inventory Management is Enabled](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3745415.html).

## CyberSource Decision Manager Fields for Web Store Orders {#bridgehead_N3691598}

As of the 2012.1 endpoint, sales order records include the following fields to be used in conjunction with CyberSource Decision Manager for third party Web store orders.

-   shopperipaddress - captures the shopper's IP address, passes it to a newly created or updated sales order, and sends it to CyberSource with the authorization request.
    

Important:

The shopperipaddress field is required for Web store orders made through SOAP web services. A SOAP web services order that does not include a value for this field is treated as an internal (MOTO) order.

-   saveonauthdecline - boolean that indicates whether to save Web store orders that receive a credit card authorization decline.
    
    -   When value is set to True, declined order is saved and placed on Payment Hold for further review. (This is the default.)
        
    -   When value is set to False, declined order is not saved, and the shopper can retry submitting the order with a different payment method.
        

The following code illustrates how to add a Web store order when CyberSource Decision Manager is in use:

## SOAP Request {#bridgehead_N3691664}

          `<add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <record externalId="Melon16973236" xsi:type="ns6:SalesOrder" xmlns:ns6="urn:sales_2017_1.transactions.webservices.netsuite.com">                <ns6:customForm internalId="109" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"/>                <ns6:entity internalId="102" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>                <ns6:paymentMethod internalId="8" type="paymentMethod" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com"/>                <ns6:shopperIpAddress xsi:type="xsd:string">167.216.129.12</ns6:shopperIpAddress>                <ns6:saveOnAuthDecline xsi:type="xsd:boolean">true</ns6:saveOnAuthDecline>                <ns6:ccNumber xsi:type="xsd:string">4111111111111111</ns6:ccNumber>                <ns6:ccExpireDate xsi:type="xsd:dateTime">2012-02-02T19:41:13.702Z</ns6:ccExpireDate>                <ns6:ccName xsi:type="xsd:string">James James</ns6:ccName>                <ns6:creditCardProcessor internalId="4" xsi:type="ns10:RecordRef" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com"/>                <ns6:getAuth xsi:type="xsd:boolean">true</ns6:getAuth>                <ns6:itemList replaceAll="false" xsi:type="ns6:SalesOrderItemList">                   <ns6:item xsi:type="ns6:SalesOrderItem">                      <ns6:item internalId="447" xsi:type="ns11:RecordRef" xmlns:ns11="urn:core_2017_1.platform.webservices.netsuite.com"/>                      <ns6:quantity xsi:type="xsd:double">2.0</ns6:quantity>                   </ns6:item>                   <ns6:item xsi:type="ns6:SalesOrderItem">                      <ns6:item internalId="451" xsi:type="ns12:RecordRef" xmlns:ns12="urn:core_2017_1.platform.webservices.netsuite.com"/>                      <ns6:quantity xsi:type="xsd:double">2.0</ns6:quantity>                   </ns6:item>                </ns6:itemList>             </record>          </add>` 
        

For more information about using CyberSource Decision Manager, see [CyberSource](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1573308.html). Specificall, read [Set Up Decision Manager for SOAP Web Services Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1573308.html#procedure_N1573758).

### Related Topics

-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Usage Notes for Transaction Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3658677.html)
-   [Transaction Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659492.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [CyberSource](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1573308.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
