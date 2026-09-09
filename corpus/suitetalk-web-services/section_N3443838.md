---
id: "section_N3443838"
type: "section"
title: "Deleting All Lines on a Sublist"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Sublists in SOAP Web Services > Deleting All Lines on a Sublist"
parent: "section_N3439908"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3443838.html"
anchors: ["bridgehead_3705118466", "bridgehead_3705430117", "bridgehead_3705123752", "bridgehead_3705124377"]
sha256: "9b4735ac79346840856b511a6649dd429f3c7b0ab6ae1e5240bbc9c2a59c6955"
---

This sample shows how to delete all addresses from the Address sublist on a customer record (CustomerAddressbookList).

## Java {#bridgehead_3705118466}

          `Customer update = new Customer(); update.setInternalId(c.getInternalId()); cabl = new CustomerAddressbookList(); cabl.setAddressbook(new CustomerAddressbook[0]); cabl.setReplaceAll(true); update.setAddressbookList(cabl);` 
        

## SOAP {#bridgehead_3705430117}

          `<update xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <record internalId="724" xsi:type="ns1:Customer" xmlns:ns1="urn:relationships_2017_1.lists.webservices.netsuite.com">                <ns1:addressbookList replaceAll="true" xsi:type="ns1:CustomerAddressbookList"/>             </record>          </update>` 
        

The next sample shows how to delete all line items from the Item sublist (OpportunityItemList) on an opportunity record.

## Java {#bridgehead_3705123752}

          `Opportunity update = new Opportunity(); update.setInternalId(opp.getInternalId()); update.setItemList(new OpportunityItemList(new OpportunityItem[0], true));` 
        

## SOAP {#bridgehead_3705124377}

          `<update xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <record internalId="6147" xsi:type="ns1:Opportunity" xmlns:ns1="urn:sales_2017_1.transactions.webservices.netsuite.com">                <ns1:itemList replaceAll="true" xsi:type="ns1:OpportunityItemList"/>             </record>          </update>` 
        

### Related Topics

-   [Sublists in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439908.html)
-   [Updating Sublists in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3441570.html)
-   [Sublist Line Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3443715.html)
-   [Searching a Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3443977.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
