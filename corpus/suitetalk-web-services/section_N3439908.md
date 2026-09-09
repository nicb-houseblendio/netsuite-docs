---
id: "section_N3439908"
type: "section"
title: "Sublists in SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Sublists in SOAP Web Services"
parent: "chapter_N3428523"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439908.html"
anchors: []
sha256: "ca7e7703e769890fb7480794921200e73b4df59235ae85dc9eda41481db793ce"
---

Most records in NetSuite include sublists, which generally contain a list of references to other records. This figure shows the Expenses sublist on the check record. Notice that this sublist includes one line in the Expenses sublist.

Note:

For general information about sublists in NetSuite, see [Record Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4309567650.html)

![The Expenses sublist in the UI.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteTalkWebServices/ExpensesSublist.png)

In SOAP web services, sublists are represented in a record's schema definition by its **List** elements. Custom sublists are not available in SOAP web services.

Note:

Except for the customFieldList element (which contains a record's custom fields), all other elements that end in **List** represent a record's sublists.

The following is a portion of the schema for the Check record. (Although the XSD shown below describes the Items sublist on the check record, the same pattern for defining sublists applies to all sublists on all records.)

Notice that the sublists on the check record include the Expenses sublist, the Items sublist, and the Landed Costs sublist (not shown in the figure above because the Landed Costs feature is not enabled in the account).

          `<complexType name="Check">         <complexContent>             <extension base="platformCore:Record">                 <sequence>                     <element name="createdDate" type="xsd:dateTime" minOccurs="0"/>                     <element name="address" type="xsd:string" minOccurs="0"/>                     <element name="subsidiary" type="platformCore:RecordRef" minOccurs="0"/>          ........                     <element name=" expenseList " type="tranBank:CheckExpenseList" minOccurs="0"/>                     <element name=" itemList " type="tranBank:CheckItemList" minOccurs="0"/>                     <element name=" landedCostsList " type="tranBank:CheckLandedCostList" minOccurs="0"/>                     <element name="billPay" type="xsd:boolean" minOccurs="0"/>                     <element name="customFieldList" type="platformCore:CustomFieldList" minOccurs="0"/>                 </sequence>               </extension>         </complexContent>     </complexType>` 
        

The **itemList** element (listed above) is of type **CheckItemList**, which is defined in the **CheckItem** complex type (defined in transactions.bank.xsd). The **CheckItem** type (shown below) includes all the properties that can be set for the Item sublist on the check record. Also notice the replaceAll attribute in CheckItemList. You will set the value of replaceAll to true or false depending on whether you are working with keyed sublists or non-keyed sublists. See [Updating Sublists in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3441570.html) for details.

          `<complexType name=" CheckItem ">         <sequence>             <element name="item" type="platformCore:RecordRef" minOccurs="0"/>             <element name="vendorName" type="xsd:string" minOccurs="0"/>       ....                    <element name="line" type="xsd:long" minOccurs="0"/>             <element name="location" type="platformCore:RecordRef" minOccurs="0"/>             <element name="isBillable" type="xsd:boolean" minOccurs="0"/>             <element name="customFieldList" type="platformCore:CustomFieldList" minOccurs="0"/>         </sequence>     </complexType>     <complexType name=" CheckItemList ">         <sequence>             <element name="item" type="tranBank:CheckItem" minOccurs="0" maxOccurs="unbounded"/>         </sequence>         <attribute name=" replaceAll " type="xsd:boolean" default="true"/>     </complexType>` 
        

### Related Topics

-   [Records in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3428663.html)
-   [Fields in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436475.html)
-   [Forms in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439676.html)
-   [Updating Sublists in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3441570.html)
-   [Sublist Line Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3443715.html)
-   [Deleting All Lines on a Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3443838.html)
-   [Searching a Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3443977.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
