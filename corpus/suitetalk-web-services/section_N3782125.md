---
id: "section_N3782125"
type: "section"
title: "Promotion Code"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Marketing Records > Promotion Code"
parent: "chapter_N3775421"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3782125.html"
anchors: ["bridgehead_N3782143", "bridgehead_N3782383", "bridgehead_N3782420", "bridgehead_3820243978", "bridgehead_N29043581", "bridgehead_N29043521"]
sha256: "cd01f0e17992ddad9dd3dec0cadfad3093e57ab81af33c940183c7f50e6cb299"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Promotion Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_76112913770.html).

Promotions enable you to track the source of revenue and to offer discounts in the form of coupons. Each promotion has a promotion code that can be applied to transactions and campaigns.

The promotion code record is defined in the [listMkt (marketing)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/marketing.xsd) XSD.

For information about working with this record in the UI, see [Selling with Promotion Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1044239.html).

## Supported Operations {#bridgehead_N3782143}

The following operations can be used with promotion code records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3782383}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [promotion code](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/promotioncode.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3782420}

Warning:

Line discount promotions are not compatible with 2009.2 and earlier endpoints. If you want to use these with SOAP web services, you must upgrade to the 2010.1 or later endpoint.

## Code Sample {#bridgehead_3820243978}

The following sample shows how to add a promotion code record to NetSuite.

## Java {#bridgehead_N29043581}

          `public void addPromotionCode()throws RemoteException    {       //This operation requires a valid session       this.login(true);              String readStr = "";       PromotionCode pc = new PromotionCode();         _console.writeLn("\nPlease enter promotion name: ");       readStr = _console.readLn();       pc.setCode(readStr);              _console.writeLn("\nPlease enter description : ");       readStr = _console.readLn();       pc.setDescription(readStr);              pc.setIsInactive(new Boolean(false));              _console.writeLn("\nPlease enter the discount item internal ID: ");       readStr = _console.readLn();       RecordRef discount = new RecordRef();       discount.setType(RecordType.discountItem);       discount.setInternalId(readStr);       pc.setDiscount(discount);              //pc.setRate(String rate) //required if discount item not specified       //pc.setDiscountType(Boolean discountType) //required if discount item not specified       _console.writeLn("Do you want to apply code to first sale only or all sales?");              while(true)       {          _console.writeLn("\nEnter 1 for First Sale Only, 2 for All Sales.");          readStr = _console.readLn();          PromotionCodeApplyDiscountTo applyDiscountTo = null;                    if(readStr.equalsIgnoreCase("1"))          {             applyDiscountTo = PromotionCodeApplyDiscountTo._firstSaleOnly;             pc.setApplyDiscountTo(applyDiscountTo);             break;          }          if(readStr.equalsIgnoreCase("2"))          {             applyDiscountTo = PromotionCodeApplyDiscountTo._allSales;             pc.setApplyDiscountTo(applyDiscountTo);             break;          }       }              Calendar startDate = Calendar.getInstance();       Calendar endDate = Calendar.getInstance();              _console.writeLn("Enter promotion code starting day.");       readStr = _console.readLn();       int day = Integer.parseInt(readStr);              _console.writeLn("Enter promotion code starting month (1-12).");       readStr = _console.readLn();       int month = Integer.parseInt(readStr);              //January=0       startDate.set(2009, month-1, day);       pc.setStartDate(startDate);              _console.writeLn("Enter promotion code ending day.");       readStr = _console.readLn();       day = Integer.parseInt(readStr);              _console.writeLn("Enter promotion code ending month (1-12).");       readStr = _console.readLn();       month = Integer.parseInt(readStr);         endDate.set(2009, month-1, day);                 pc.setEndDate(endDate);              pc.setIsPublic(new Boolean(true));       pc.setExcludeItems(new Boolean(false));                 WriteResponse writeRes = _port.add(pc);       boolean success = writeRes.getStatus().isIsSuccess();       if (success)        {          _console.writeLn("\nPromotion Code created successfully.");          RecordRef _ref = (RecordRef)(writeRes.getBaseRef());          _console.writeLn("Internal ID: " + _ref.getInternalId());       }        else        {          _console.error(getStatusDetails(writeRes.getStatus()));       }       }` 
        

## SOAP Request {#bridgehead_N29043521}

          `<soapenv:Body>       <platformMsgs:add           xmlns:soapenc="http://schemas.xmlsoap.org/soap/encoding/"           xmlns:listMktTyp="urn:types.marketing_2017_1.lists.webservices.netsuite.com"           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"           xmlns:platformMsgs="urn:messages_2017_1.platform.webservices.netsuite.com"           xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"           xmlns:xs="http://www.w3.org/2001/XMLSchema"           xmlns:s0="urn:marketing_2017_1.lists.webservices.netsuite.com"           xmlns:s1="urn:sales_2017_1.transactions.webservices.netsuite.com">          <platformMsgs:record xsi:type="s0:PromotionCode">             <s0:code>Any Promo Code</s0:code>             <s0:isInactive>false</s0:isInactive>             <s0:discount internalId="28" />             <s0:applyDiscountTo>_firstSaleOnly</s0:applyDiscountTo>             <s0:startDate>2009-01-09T23:23:38.787Z</s0:startDate>             <s0:endDate>2009-01-16T18:23:52.000Z</s0:endDate>             <s0:isPublic>true</s0:isPublic>             <s0:excludeItems>false</s0:excludeItems>          </platformMsgs:record>       </platformMsgs:add>    </soapenv:Body> </soapenv:Envelope>` 
        

### Related Topics

-   [Marketing Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3775421.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
