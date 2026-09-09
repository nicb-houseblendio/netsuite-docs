---
id: "section_N3705423"
type: "section"
title: "Working with Matrix Items in SOAP web services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Items > Working with Matrix Items in SOAP web services"
parent: "chapter_N3704574"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705423.html"
anchors: ["bridgehead_N3705587", "bridgehead_N3705746", "bridgehead_N3705770", "bridgehead_N3705821", "bridgehead_N3705837", "bridgehead_N3707560", "bridgehead_N3707591", "bridgehead_N3707608", "bridgehead_N28616881", "bridgehead_N28616941", "bridgehead_N3707639", "bridgehead_3820188957"]
sha256: "4e94441aa9e96e48ea300473b4ab5acf12776d5235ab3227d0be7066720dc0b6"
---

Before working with matrix items in SOAP web services, you must first enable the Matrix Item feature in your NetSuite account. To enable this feature go to _Setup > Company > Enable Features_, on the Items & Inventory subtab, check the Matrix Items box.

This section covers the following topics:

-   [Item Types that Support Matrix Options](#bridgehead_N3705587)
    
-   [Creating a Parent Matrix Item](#bridgehead_N3705746)
    
-   [Creating a Child Matrix Item](#bridgehead_N3705770)
    
-   [Specifying Matrix Options](#bridgehead_N3705821)
    
-   [Matrix Dimensions](#bridgehead_N3705837)
    
-   [Updating Child and Parent Matrix Items](#bridgehead_N3707560)
    
-   [Deleting Child and Parent Matrix Items](#bridgehead_N3707591)
    
-   [Matrix Item Code Sample](#bridgehead_N3707608)
    

Note:

For general information about the matrix items feature, see [Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227654.html).

## Item Types that Support Matrix Options {#bridgehead_N3705587}

You can use SOAP web services to create matrix items for the following record types:

-   Inventory Item
    
-   Lot Numbered Inventory Item
    
-   Serialized Inventory Item
    
-   Non-Inventory Item for Sale
    
-   Non-Inventory Item for Resale
    
-   Non-Inventory Item for Purchase
    
-   Service Item for Sale
    
-   Service Item for Resale
    
-   Service Item for Purchase
    
-   Other Charge Item for Sale
    
-   Other Charge Item for Resale
    
-   Other Charge Item for Purchase
    

Note that item types that supports matrix options includes the following elements:

-   A matrixType enum field which can take the value of either \_parent or \_child to indicate if the submitted record is a parent or child matrix item. See [Creating a Parent Matrix Item](#bridgehead_N3705746).
    
-   A parent (Subitem of) field that points to a matrix parent item and populates the MatrixOption list. See [Creating a Child Matrix Item](#bridgehead_N3705770).
    
-   A MatrixOptionList element (similar to the Matrix subtab on the UI). This element is an array of customFieldList of type select to populate matrix options on the child record. Users can specify only one value per matrix option field.
    

## Creating a Parent Matrix Item {#bridgehead_N3705746}

Users must set the matrixType field if they want to specify an item as either a parent or child matrix item.

Note:

This is a deviation from the UI behavior. In the UI you cannot create a parent matrix item without selecting the child options, however, in SOAP web services this is possible.

## Creating a Child Matrix Item {#bridgehead_N3705770}

If users have already setup matrix item options in their account, they can proceed with creating child matrix items. As opposed to the UI where selecting matrix options on the parent will result in creating the matrix children, in SOAP web services the user has to add each child matrix item separately.

The user must set the RecordRef of the parent (Subitem of) field and specify one or more matrix options for the matrix child item record. Note that the parent item must have the is MatrixParent field set to true, otherwise the following error is thrown:

Error code = INVALID\_MATRIX\_PARENT

Error message = Item {1} is not a parent matrix item.

Users can set also set the externalId field to submit parent matrix item data and associate the child matrix items with the parent in a single addList request in SOAP web services.

Important:

A maximum of 2000 children are permitted for a parent item.

## Specifying Matrix Options {#bridgehead_N3705821}

A call to getCustomization('itemOptionCustomField') can be used to return valid matrix option fields and values. A get on the parent matrix item returns only the matrix options that have been used. Not all possible options are returned.

## Matrix Dimensions {#bridgehead_N3705837}

After the first child is created, the dimensions for the matrix item are set and can not be changed. For example, if users creates a large, blue dress as the first child matrix item, they cannot subsequently create a dress that has any property other than size and color. A small, red, cotton dress will not be a valid option.

If users try to add a new child matrix with options that already exists for the parent, they will receive an error.

## Updating Child and Parent Matrix Items {#bridgehead_N3707560}

Users cannot update child matrix items through the parent record. Users must submit updates for child items individually.

For example, in SOAP web services, updating parent item values for the Asset Account, Cost of Goods Sold (COGS) account, or Income Account fields does not automatically update child item field values. You need to set these values for each child item row. The system does not enforce that child item values match the parent item values for these fields, so you need to ensure that they match yourself.

Also note that the following error is thrown if users attempt to update an existing item to make it a parent.

          `Error Code = USER_ERROR Error Message = You can not change an existing item to make it a parent matrix item {1}.` 
        

Note:

The values that are returned in MatrixOptionList are read-only after the child matrix item is added.

## Deleting Child and Parent Matrix Items {#bridgehead_N3707591}

In SOAP web services users cannot delete a parent item if it has children. They must delete the child items individually before deleting the parent.

A check for child matrix items occurs on a request to delete a parent matrix item. If no children exist, the parent item is deleted. If children do exist, an error is returned stating that the parent has child items.

## Matrix Item Code Sample {#bridgehead_N3707608}

## SOAP Request {#bridgehead_N28616881}

          `<?xml version="1.0" encoding="UTF-8"?>    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">        <soapenv:Body>            <addList xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <record externalId="parentSweater" xsi:type="ns1:InventoryItem" xmlns:ns1="urn:accounting_2017_1.lists.webservices.netsuite.com">                    <ns1:matrixType xsi:type="ns2:ItemMatrixType" xmlns:ns2="urn:types.accounting_2017_1.lists.webservices.netsuite.com">_parent</ns1:matrixType>                    <ns1:itemId xsi:type="xsd:string">sweater</ns1:itemId>                </record>                <record externalId="sweater-Red-Large" xsi:type="ns3:InventoryItem" xmlns:ns3="urn:accounting_2017_1.lists.webservices.netsuite.com">                    <ns3:matrixType xsi:type="ns4:ItemMatrixType" xmlns:ns4="urn:types.accounting_2017_1.lists.webservices.netsuite.com">_child</ns3:matrixType>                    <ns3:itemId xsi:type="xsd:string">sweater-Red-Large</ns3:itemId>                    <ns3:parent externalId="parentSweater" xsi:type="ns5:RecordRef" xmlns:ns5="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns3:matrixOptionList xsi:type="ns3:MatrixOptionList">                        <ns3:matrixOption scriptId="CUSTITEM_COLOR" xsi:type="ns6:SelectCustomFieldRef" xmlns:ns6="urn:core_2017_1.platform.webservices.netsuite.com">                            <ns6:value internalId="1" typeId="1" xsi:type="ns6:ListOrRecordRef">                                <ns6:name xsi:type="xsd:string">Red</ns6:name>                            </ns6:value>                        </ns3:matrixOption>                        <ns3:matrixOption scriptId="CUSTITEM_SIZE" xsi:type="ns7:SelectCustomFieldRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com">                            <ns7:value internalId="2" typeId="2" xsi:type="ns7:ListOrRecordRef">                                <ns7:name xsi:type="xsd:string">Large</ns7:name>                            </ns7:value>                        </ns3:matrixOption>                    </ns3:matrixOptionList>                </record>                <record externalId="sweater-Green-Small" xsi:type="ns8:InventoryItem" xmlns:ns8="urn:accounting_2017_1.lists.webservices.netsuite.com">                    <ns8:matrixType xsi:type="ns9:ItemMatrixType" xmlns:ns9="urn:types.accounting_2017_1.lists.webservices.netsuite.com">_child</ns8:matrixType>                    <ns8:itemId xsi:type="xsd:string">sweater-Green-Small</ns8:itemId>                    <ns8:parent externalId="parentSweater" xsi:type="ns10:RecordRef" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns8:matrixOptionList xsi:type="ns8:MatrixOptionList">                        <ns8:matrixOption scriptId="CUSTITEM_COLOR" xsi:type="ns11:SelectCustomFieldRef" xmlns:ns11="urn:core_2017_1.platform.webservices.netsuite.com">                            <ns11:value internalId="2" typeId="1" xsi:type="ns11:ListOrRecordRef">                                <ns11:name xsi:type="xsd:string">Green</ns11:name>                            </ns11:value>                        </ns8:matrixOption>                        <ns8:matrixOption scriptId="CUSTITEM_SIZE" xsi:type="ns12:SelectCustomFieldRef" xmlns:ns12="urn:core_2017_1.platform.webservices.netsuite.com">                            <ns12:value internalId="3" typeId="2" xsi:type="ns12:ListOrRecordRef">                                <ns12:name xsi:type="xsd:string">Small</ns12:name>                            </ns12:value>                        </ns8:matrixOption>                    </ns8:matrixOptionList>                </record>                <record externalId="sweater-Blue-Large" xsi:type="ns13:InventoryItem" xmlns:ns13="urn:accounting_2017_1.lists.webservices.netsuite.com">                    <ns13:matrixType xsi:type="ns14:ItemMatrixType" xmlns:ns14="urn:types.accounting_2017_1.lists.webservices.netsuite.com">_child</ns13:matrixType>                    <ns13:itemId xsi:type="xsd:string">sweater-Blue-Large</ns13:itemId>                    <ns13:parent externalId="parentSweater" xsi:type="ns15:RecordRef" xmlns:ns15="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns13:matrixOptionList xsi:type="ns13:MatrixOptionList">                        <ns13:matrixOption scriptId="CUSTITEM_COLOR" xsi:type="ns16:SelectCustomFieldRef" xmlns:ns16="urn:core_2017_1.platform.webservices.netsuite.com">                            <ns16:value internalId="3" typeId="1" xsi:type="ns16:ListOrRecordRef">                                <ns16:name xsi:type="xsd:string">Blue</ns16:name>                            </ns16:value>                        </ns13:matrixOption>                        <ns13:matrixOption scriptId="CUSTITEM_SIZE" xsi:type="ns17:SelectCustomFieldRef" xmlns:ns17="urn:core_2017_1.platform.webservices.netsuite.com">                            <ns17:value internalId="2" typeId="2" xsi:type="ns17:ListOrRecordRef">                                <ns17:name xsi:type="xsd:string">Large</ns17:name>                            </ns17:value>                        </ns13:matrixOption>                    </ns13:matrixOptionList>                </record>                <record externalId="sweater-Red-Small" xsi:type="ns18:InventoryItem" xmlns:ns18="urn:accounting_2017_1.lists.webservices.netsuite.com">                    <ns18:matrixType xsi:type="ns19:ItemMatrixType" xmlns:ns19="urn:types.accounting_2017_1.lists.webservices.netsuite.com">_child</ns18:matrixType>                    <ns18:itemId xsi:type="xsd:string">sweater-Red-Small</ns18:itemId>                    <ns18:parent externalId="parentSweater" xsi:type="ns20:RecordRef" xmlns:ns20="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns18:matrixOptionList xsi:type="ns18:MatrixOptionList">                        <ns18:matrixOption scriptId="CUSTITEM_COLOR" xsi:type="ns21:SelectCustomFieldRef" xmlns:ns21="urn:core_2017_1.platform.webservices.netsuite.com">                            <ns21:value internalId="1" typeId="1" xsi:type="ns21:ListOrRecordRef">                                <ns21:name xsi:type="xsd:string">Red</ns21:name>                            </ns21:value>                        </ns18:matrixOption>                        <ns18:matrixOption scriptId="CUSTITEM_SIZE" xsi:type="ns22:SelectCustomFieldRef" xmlns:ns22="urn:core_2017_1.platform.webservices.netsuite.com">                            <ns22:value internalId="3" typeId="2" xsi:type="ns22:ListOrRecordRef">                                <ns22:name xsi:type="xsd:string">Small</ns22:name>                            </ns22:value>                        </ns18:matrixOption>                    </ns18:matrixOptionList>                </record>                <record externalId="sweater-Green-Large" xsi:type="ns23:InventoryItem" xmlns:ns23="urn:accounting_2017_1.lists.webservices.netsuite.com">                    <ns23:matrixType xsi:type="ns24:ItemMatrixType" xmlns:ns24="urn:types.accounting_2017_1.lists.webservices.netsuite.com">_child</ns23:matrixType>                    <ns23:itemId xsi:type="xsd:string">sweater-Green-Large</ns23:itemId>                    <ns23:parent externalId="parentSweater" xsi:type="ns25:RecordRef" xmlns:ns25="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns23:matrixOptionList xsi:type="ns23:MatrixOptionList">                        <ns23:matrixOption scriptId="CUSTITEM_COLOR" xsi:type="ns26:SelectCustomFieldRef" xmlns:ns26="urn:core_2017_1.platform.webservices.netsuite.com">                            <ns26:value internalId="2" typeId="1" xsi:type="ns26:ListOrRecordRef">                                <ns26:name xsi:type="xsd:string">Green</ns26:name>                            </ns26:value>                        </ns23:matrixOption>                        <ns23:matrixOption scriptId="CUSTITEM_SIZE" xsi:type="ns27:SelectCustomFieldRef" xmlns:ns27="urn:core_2017_1.platform.webservices.netsuite.com">                            <ns27:value internalId="2" typeId="2" xsi:type="ns27:ListOrRecordRef">                                <ns27:name xsi:type="xsd:string">Large</ns27:name>                            </ns27:value>                        </ns23:matrixOption>                    </ns23:matrixOptionList>                </record>                <record externalId="sweater-Blue-Small" xsi:type="ns28:InventoryItem" xmlns:ns28="urn:accounting_2017_1.lists.webservices.netsuite.com">                    <ns28:matrixType xsi:type="ns29:ItemMatrixType" xmlns:ns29="urn:types.accounting_2017_1.lists.webservices.netsuite.com">_child</ns28:matrixType>                    <ns28:itemId xsi:type="xsd:string">sweater-Blue-Small</ns28:itemId>                    <ns28:parent externalId="parentSweater" xsi:type="ns30:RecordRef" xmlns:ns30="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns28:matrixOptionList xsi:type="ns28:MatrixOptionList">                        <ns28:matrixOption scriptId="CUSTITEM_COLOR" xsi:type="ns31:SelectCustomFieldRef" xmlns:ns31="urn:core_2017_1.platform.webservices.netsuite.com">                            <ns31:value internalId="3" typeId="1" xsi:type="ns31:ListOrRecordRef">                                <ns31:name xsi:type="xsd:string">Blue</ns31:name>                            </ns31:value>                        </ns28:matrixOption>                        <ns28:matrixOption scriptId="CUSTITEM_SIZE" xsi:type="ns32:SelectCustomFieldRef" xmlns:ns32="urn:core_2017_1.platform.webservices.netsuite.com">                            <ns32:value internalId="3" typeId="2" xsi:type="ns32:ListOrRecordRef">                         <ns32:name xsi:type="xsd:string">Small</ns32:name>                            </ns32:value>                        </ns28:matrixOption>                    </ns28:matrixOptionList>                </record>            </addList>        </soapenv:Body>    </soapenv:Envelope>` 
        

## Java {#bridgehead_N28616941}

          `/** Create Sweaters as matrix items. * First create the parent - no matrix properties except "Matrix Type" is Parent * Second create the matrix children with a combination of sizes and colors. * This can be done in a single addList (as shown).  */ //Define mrr method public static RecordRef mrr(String internalId)  {   RecordRef toRet = new RecordRef();   toRet.setInternalId(internalId);   return toRet;  }   // Define makeListOrRecordRef method public static ListOrRecordRef makeListOrRecordRef(String sTypeId, String internalId, String sName)  {   ListOrRecordRef toRet = new ListOrRecordRef();   toRet.setInternalId(internalId);   toRet.setName(sName);   toRet.setTypeId(sTypeId);   return toRet;  }   public void testMatrixSample() throws Exception    { // Color is a Custom List of TypeId/RecType 1 that has already been created. 1,2,3 represent the // internalIds of Red, Green, Blue ListOrRecordRef[] colorArray = new    ListOrRecordRef[] {makeListOrRecordRef("1","1","Red"), makeListOrRecordRef("1","2","Green"),    makeListOrRecordRef("1","3","Blue")}; // Representing red, green and blue // Size is a CustomList of TypeId/RecType 2 that has already been created ListOrRecordRef[] sizeArray = new ListOrRecordRef[]{makeListOrRecordRef("2","2","Large"),makeListOrRecordRef("2","3","Small")};   //Representing large and small       InventoryItem[] toSubmit = new InventoryItem[1+colorArray.length*sizeArray.length];       toSubmit[0] = new InventoryItem();       toSubmit[0].setExternalId("parentSweater");       toSubmit[0].setItemId("sweater");       toSubmit[0].setMatrixType(ItemMatrixType._parent);       // set other fields on the Parent        for (int i=0;i<colorArray.length*sizeArray.length;i++)       {          toSubmit[i+1] = new InventoryItem();          toSubmit[i+1].setMatrixType(ItemMatrixType._child);          // mrr Creates a recordRef given an internal and externalId, the latter of which we specify.          // This makes it so we can submit all the records at one time          toSubmit[i+1].setParent(mrr((String)null,"parentSweater"));          // "sweater-large-red","sweater-large-green"...          toSubmit[i+1].setItemId("sweater-"+colorArray[i%3].getName() + "-" +              sizeArray[i % 2].getName());          // set externalId so it's easier to find later          toSubmit[i+1].setExternalId(toSubmit[i+1].getItemId());          // CUSTITEM_COLOR,SIZE are the names of the Item Custom Fields, applied to          //InventoryItem that were setup as a Matrix types.          SelectCustomFieldRef colorRef = new SelectCustomFieldRef();          colorRef.setScriptId("CUSTITEM_COLOR");          colorRef.setValue(colorArray[i%3]);          SelectCustomFieldRef sizeRef = new SelectCustomFieldRef();          sizeRef.setScriptId("CUSTITEM_SIZE");          sizeRef.setValue(sizeArray[i%2]);          toSubmit[i+1].setMatrixOptionList(new MatrixOptionList(new             SelectCustomFieldRef[]{colorRef,sizeRef}));                      // Set other matrix item child files          //....       }         WriteResponseList wr = c.getPort().addList(toSubmit);    }` 
        

## Working with the Pricing Matrix {#bridgehead_N3707639}

The following method takes an InventoryItem record and sets its pricing matrix. It sets the base price at quantity 0. If an invalid price was entered (a non-numeric value), it does not set the pricing matrix.

## Sample Java Code {#bridgehead_3820188957}

          `private void createPricingMatrix(InventoryItem item) {    _console.write("\nPlease enter the base price: ");    String priceString = _console.readLn();    Price[] prices = new Price[1];    prices[0] = new Price();    try    {    prices[0].setValue(Double.valueOf(priceString));    prices[0].setQuantity(null);     PriceList priceList = new PriceList();    priceList.setPrice(prices);     Pricing[] pricing = new Pricing[1];    pricing[0] = new Pricing();    pricing[0].setPriceList(priceList);    pricing[0].setDiscount(null);    RecordRef priceLevel = new RecordRef();    priceLevel.setInternalId(BASE_PRICE_LEVEL_INTERNAL_ID);    priceLevel.setType(RecordType.priceLevel);    pricing[0].setPriceLevel(priceLevel);    RecordRef currUSD = new RecordRef();    currUSD.setInternalId("1");    pricing[0].setCurrency(currUSD);     PricingMatrix pricingMatrix = new PricingMatrix();    pricingMatrix.setPricing(pricing);    pricingMatrix.setReplaceAll(false);     item.setPricingMatrix(pricingMatrix);    }    catch (NumberFormatException e)    {       _console.error("\nInvalid base price entered: " + priceString + ".            Proceed creating item without setting pricing matrix.");    } }` 
        

### Related Topics

-   [Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3704574.html)
-   [Usage Notes for Item Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705128.html)
-   [Shared Field Definitions for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3707811.html)
-   [Item Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3713653.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
