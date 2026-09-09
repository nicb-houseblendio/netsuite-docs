---
id: "section_N3687114"
type: "section"
title: "Paycheck Journal"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Paycheck Journal"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3687114.html"
anchors: ["bridgehead_N3687158", "bridgehead_N3687336", "bridgehead_N3687373", "bridgehead_N3687381", "bridgehead_N3687444", "bridgehead_N3687457", "bridgehead_N3687469", "bridgehead_N3687486", "bridgehead_N3687498", "bridgehead_N3687513", "bridgehead_N3687525"]
sha256: "2f6e930765aa308e9e236eb5eec7749af9aa915416466e18774b5464f0e1727d"
---

The paycheck journal transaction serves as a payroll interface for SOAP web services integrations with external payroll systems. This transaction is similar to the paycheck transaction used by SuitePeople US Payroll. However, unlike a paycheck, a paycheck journal cannot issue a check drawn on an account. On its own, a paycheck journal functions as a journal entry; it records accounting impact.

This transaction is available when the Paycheck Journal feature is enabled at Setup > Company > Enable Features, on the Employees subtab.

For more details about this type of transaction, see [Paycheck Journal Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N969418.html).

The paycheck journal record is defined in the [tranEmp (employees)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/employees.xsd) XSD.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Supported Operations {#bridgehead_N3687158}

The following operations can be used with paycheck journal records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3687336}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [paycheck journal](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/paycheckjournal.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3687373}

## Working with Paycheck Journal Sublists {#bridgehead_N3687381}

This record includes the following sublists:

-   PaycheckJournalCompanyContributionList
    
-   PaycheckJournalDeductionList
    
-   PaycheckJournalEmployeeTaxList
    
-   PaycheckJournalCompanyTaxList
    
-   PaycheckJournalEarningList
    
-   CustomFieldList
    

The CustomFieldList sublist stores values for custom transaction body fields added to a paycheck journal. Note that each of the other sublists can include its own CustomFieldList to store values for custom transaction column fields.

## Sample Code {#bridgehead_N3687444}

The following examples add a paycheck journal transaction.

## SOAP Request {#bridgehead_N3687457}

          `/*    <soapenv:Body>            <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <record externalId="Grape14276260" xsi:type="ns6:PaycheckJournal" xmlns:ns6="urn:employees_2017_1.transactions.webservices.netsuite.com">                    <ns6:employee internalId="4" type="employee" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns6:tranDate xsi:type="xsd:dateTime">2012-06-10T14:33:56.451Z</ns6:tranDate>                    <ns6:account internalId="4" type="account" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns6:earningList replaceAll="false" xsi:type="ns6:PaycheckJournalEarningList">                        <ns6:paycheckJournalEarning xsi:type="ns6:PaycheckJournalEarning">                            <ns6:payrollItem internalId="102" type="payrollItem" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com"/>                            <ns6:amount xsi:type="xsd:double">20.0</ns6:amount>                        </ns6:paycheckJournalEarning>                        <ns6:paycheckJournalEarning xsi:type="ns6:PaycheckJournalEarning">                            <ns6:payrollItem internalId="102" type="payrollItem" xsi:type="ns10:RecordRef" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com"/>                            <ns6:amount xsi:type="xsd:double">20.0</ns6:amount>                        </ns6:paycheckJournalEarning>                    </ns6:earningList>                </record>            </add>        </soapenv:Body>      */` 
        

## Java {#bridgehead_N3687469}

          `public void addPaycheckJournalSample() throws Exception     {        // This operation requires a valid session        this.login(true);                PaycheckJournal pj =  new PaycheckJournal();                RecordRef rrEmployee =  new RecordRef();        rrEmployee.setType(RecordType.employee);        rrEmployee.setInternalId("4");                pj.setEmployee(rrEmployee);                RecordRef rrAccount =  new RecordRef();        rrAccount.setType(RecordType.account);        rrAccount.setInternalId("5");                 pj.setAccount(rrAccount);                  Calendar c  = Calendar.getInstance();         c.set(2012, 5, 10); //June 10, 2012         pj.setTranDate(c);                  //setting 2 lines of Payroll Item Earning Type         PaycheckJournalEarningList pjel =  new PaycheckJournalEarningList();         PaycheckJournalEarning[] pje =  new PaycheckJournalEarning[2];                  RecordRef rrPIEarning =  new RecordRef();         rrPIEarning.setType(RecordType.payrollItem);         rrPIEarning.setInternalId("102");                   RecordRef rrPIDeduction =  new RecordRef();         rrPIDeduction.setType(RecordType.payrollItem);         rrPIDeduction.setInternalId("103");                 pje[0] =  new PaycheckJournalEarning();         pje[0].setPayrollItem(rrPIEarning);         pje[0].setAmount(20.00);                  pje[1] =  new PaycheckJournalEarning();         pje[1].setPayrollItem(rrPIEarning);         pje[1].setAmount(20.00);                          pjel.setPaycheckJournalEarning(pje);         pj.setEarningList(pjel);                  //setting 1 line of Payroll Item Deduction Type         PaycheckJournalDeductionList pjdl =  new PaycheckJournalDeductionList();         PaycheckJournalDeduction[] pjd = new PaycheckJournalDeduction[1];         pjd[0] = new PaycheckJournalDeduction();         pjd[0].setAmount(30.00);         pjd[0].setPayrollItem(rrPIDeduction);         pjdl.setPaycheckJournalDeduction(pjd);           _port.add(pi);     }` 
        

The following examples update a paycheck journal transaction.

## SOAP Request {#bridgehead_N3687486}

          `/* get SOAP Request    <soapenv:Body>            <get xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <baseRef internalId="102" type="paycheckJournal" xsi:type="ns6:RecordRef" xmlns:ns6="urn:core_2017_1.platform.webservices.netsuite.com"/>            </get>      </soapenv:Body>    */        /* upate SOAP Request     <record externalId="Pear11044478" xsi:type="ns6:PaycheckJournal" xmlns:ns6="urn:employees_2017_1.transactions.webservices.netsuite.com">                    <ns6:currency internalId="1" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com">                        <ns7:name xsi:type="xsd:string">Canadian dollar</ns7:name>                    </ns6:currency>                    <ns6:exchangeRate xsi:type="xsd:double">1.0</ns6:exchangeRate>                    <ns6:createdDate xsi:type="xsd:dateTime">2012-07-26T07:33:41.000Z</ns6:createdDate>                    <ns6:lastModifiedDate xsi:type="xsd:dateTime">2012-07-26T07:33:41.000Z</ns6:lastModifiedDate>                    <ns6:employee internalId="4" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com">                        <ns8:name xsi:type="xsd:string">Mariah  Carey</ns8:name>                    </ns6:employee>                    <ns6:tranDate xsi:type="xsd:dateTime">2012-06-10T07:00:00.000Z</ns6:tranDate>                    <ns6:postingPeriod internalId="77" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com">                        <ns9:name xsi:type="xsd:string">Jun 2012</ns9:name>                    </ns6:postingPeriod>                    <ns6:account internalId="4" xsi:type="ns10:RecordRef" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com">                        <ns10:name xsi:type="xsd:string">Petty Cash</ns10:name>                    </ns6:account>                    <ns6:earningList replaceAll="false" xsi:type="ns6:PaycheckJournalEarningList">                        <ns6:paycheckJournalEarning xsi:type="ns6:PaycheckJournalEarning">                            <ns6:id xsi:type="xsd:long">1</ns6:id>                            <ns6:payrollItem internalId="102" xsi:type="ns11:RecordRef" xmlns:ns11="urn:core_2017_1.platform.webservices.netsuite.com">                                <ns11:name xsi:type="xsd:string">Re-Employment Service Fund</ns11:name>                            </ns6:payrollItem>                            <ns6:amount xsi:type="xsd:double">99.99</ns6:amount>                        </ns6:paycheckJournalEarning>                        <ns6:paycheckJournalEarning xsi:type="ns6:PaycheckJournalEarning">                            <ns6:id xsi:type="xsd:long">2</ns6:id>                            <ns6:payrollItem internalId="102" xsi:type="ns12:RecordRef" xmlns:ns12="urn:core_2017_1.platform.webservices.netsuite.com">                                <ns12:name xsi:type="xsd:string">Re-Employment Service Fund</ns12:name>                            </ns6:payrollItem>                            <ns6:amount xsi:type="xsd:double">20.0</ns6:amount>                        </ns6:paycheckJournalEarning>                    </ns6:earningList>                </record>    */` 
        

## Java {#bridgehead_N3687498}

          `public void updatePaycheckJournalSample() throws Exception     {        this.login(true);                       RecordRef rrPaycheck =  new RecordRef();        rrPaycheck.setInternalId("102");        rrPaycheck.setType(RecordType.paycheckJournal);                ReadResponse rr = (PaycheckJournal)_port.get(rrPaycheck);             PaycheckJournal pj = rr.getRecord();               pj.getEarningList().getPaycheckJournalEarning(0).setAmount(99.99);                      _port.update(pj);     }` 
        

The following examples do a basic search for paycheck journal transactions with a date of June 10, 2012.

## SOAP Request {#bridgehead_N3687513}

          `/*          <soapenv:Body>            <search xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <searchRecord xsi:type="ns6:TransactionSearchBasic" xmlns:ns6="urn:common_2017_1.platform.webservices.netsuite.com">                    <ns6:tranDate operator="on" xsi:type="ns7:SearchDateField" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com">                        <ns7:searchValue xsi:type="xsd:dateTime">2012-06-10T14:55:12.290Z</ns7:searchValue>                    </ns6:tranDate>                    <ns6:type operator="anyOf" xsi:type="ns8:SearchEnumMultiSelectField" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com">                        <ns8:searchValue xsi:type="xsd:string">_paycheckJournal</ns8:searchValue>                    </ns6:type>                </searchRecord>            </search>        </soapenv:Body>        */` 
        

## Java {#bridgehead_N3687525}

          `public void searchPaycheckJournal() throws Exception     {        this.login(true);          TransactionSearchBasic tsb =  new TransactionSearchBasic();        SearchEnumMultiSelectField semsf = new SearchEnumMultiSelectField();        semsf.setOperator(SearchEnumMultiSelectFieldOperator.anyOf);        semsf.setSearchValue(new String[] {"_paycheckJournal"});        tsb.setType(semsf);                SearchDateField sdf = new SearchDateField();        sdf.setOperator(SearchDateFieldOperator.on);                Calendar c =  Calendar.getInstance();        c.set(2012, 5, 10); //June 10, 2012        sdf.setSearchValue(c);                tsb.setTranDate(sdf);        sessMgr.getPort().search(tsb);     }` 
        

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
