---
id: "section_N3739999"
type: "section"
title: "Account"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Lists > Account"
parent: "chapter_N3739470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3739999.html"
anchors: ["bridgehead_N3740016", "bridgehead_N3740244", "bridgehead_N3740281", "bridgehead_4745802620", "bridgehead_4737768587", "bridgehead_4737785107", "bridgehead_4737788449"]
sha256: "095aeb07333e954707d5ca8a05d06a7047ddbbd997757a5eff547cee2593bb3b"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0902085857.html).

One of the first tasks you must complete before you can begin managing accounting in NetSuite is to set up a chart of accounts (COA).

For information about working with accounts in the UI, see [Chart of Accounts Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1439850.html).

The account record is defined in the [listAcct (accounting)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd) XSD.

## Supported Operations {#bridgehead_N3740016}

The following operations can be used with the account record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3740244}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [account](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/account.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Note:

The unit and unitstype fields are used only for statistical accounts, not other types of accounts. For general details on statistical accounts, see [Statistical Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3842142868.html).

## Usage Notes {#bridgehead_N3740281}

Currently there are no available search joins for this record.

In the 2020.2 and later endpoints, when you set the Use Account Numbers preference, the name field only includes the account name, and not the account number. When Use Account Numbers is not set, both name and displayName display only the account name. Endpoints 2020.1 and older are not affected.

| SOAP Endpoint Version | Use Account Numbers = True | Use Account Numbers = False |
| --- | --- | --- |
| name | displayName | name | displayName |
| --- | --- | --- | --- |
| 2021.1 | Account Name | Account Number + Account Name | Account Name | Account Name |
| 2020.2 | Account Name | Account Number + Account Name | Account Name | Account Name |
| 2020.1 and older | Account Number + Account Name | \- | Account Name | \- |

Saved search results that use the Name field now only display the Account Name, and not the Account Number and the Account Name.

If your integration uses the Search operation for an Account search and requires the Account Name to include the Account Number in the search results, you need to change the Name field (id: "name") to the Display Name field (id: "displayname"), before using your integration with the 2020.2 or later endpoints.

For information about the effect of the Use Account Numbers preference in the UI, see [General Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html).

## Certain Fields are Available for OneWorld Accounts Only {#bridgehead_4745802620}

The following fields are available for OneWorld accounts only:

-   accountingContext. At least one Accounting Context must exist in your account for this field to be available.
    
-   acctNumber. The Use Account Numbers accounting preference must be enabled for this field to be available.
    

Be aware of the following limitations for these fields in 2016.1 and earlier endpoints:

-   get operations on the account record return only lines that have null values for the accountingContext and acctNumber fields.
    
-   You cannot set values for the accountingContext and acctNumber fields in the localization sublist.
    

## Get Response {#bridgehead_4737768587}

The following snippet shows a SOAP response to a get request on the account record.

          `<listAcct:localizationsList>    <listAcct:accountLocalizations>       <listAcct:accountingContext internalId="2" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">          <platformCore:name>European Accounting Context</platformCore:name>       </listAcct:accountingContext>       <listAcct:acctName>France</listAcct:acctName>         <listAcct:locale>_frenchFrance</listAcct:locale>    </listAcct:accountLocalizations>       <listAcct:accountLocalizations>       <listAcct:acctName>Germany</listAcct:acctName>       <listAcct:locale>_german</listAcct:locale>    </listAcct:accountLocalizations> </listAcct:localizationsList>` 
        

## Java Update Request {#bridgehead_4737785107}

The following Java snippet uses the acctContext field in an update request.

          `Account account = new Account();  account.setInternalId("161"); AccountLocalizationsList accountLocalizationsList = new AccountLocalizationsList(); AccountLocalizations[] accountLocalizations = {new AccountLocalizations()}; accountLocalizations[0].setLocale(Language._russian); accountLocalizations[0].setAcctName("Office Expenses"); RecordRef acctContext = new RecordRef(); acctContext.setInternalId("1"); accountLocalizations[0].setAccountingContext(acctContext); accountLocalizationsList.setAccountLocalizations(accountLocalizations); account.setLocalizationsList(accountLocalizationsList);  c.updateRecord(account);` 
        

## Update Request {#bridgehead_4737788449}

The following SOAP snippet uses the acctContext field in an update request.

          `<update xmlns="urn:messages_2017_1.platform.webservices.netsuite.com>       <record internalId="161" xsi:type="ns8:Account" xmlns:ns8="urn:accounting_2017_1.lists.webservices.netsuite.com">          <ns8:localizationsList replaceAll="false" xsi:type="ns8:AccountLocalizationsList">                 <ns8:accountLocalizations xsi:type="ns8:AccountLocalizations">                    <ns8:accountingContext internalId="1" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <ns8:acctName xsi:type="xsd:string">Office Expenses</ns8:acctName>                      <ns8:locale xsi:type="ns10:Language" xmlns:ns10="urn:types.common_2017_1.platform.webservices.netsuite.com">_russian</ns8:locale>             </ns8:accountLocalizations>             </ns8:localizationsList>         </record> </update>` 
        

### Related Topics

-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3739470.html)
-   [Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3757146.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
