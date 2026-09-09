---
id: "section_N3796175"
type: "section"
title: "Setting State Values in SOAP web services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Country, State, and Language Enumerations > Setting State Values in SOAP web services"
parent: "chapter_N3784994"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3796175.html"
anchors: ["bridgehead_N3796270", "bridgehead_N3796280", "bridgehead_N3796318", "bridgehead_N3796390", "procedure_N3796409", "procedure_N3796462"]
sha256: "92620018adec52b99e6d1d38a1b971a9b8ea4f7953dbbce4b0fad508f119f8b3"
---

The WSDL does not include a State class or state enumeration values (previously defined in commonTypes.xsd in endpoints older than 2008.2). State fields now take any of the string values defined in the **Short Name** column on the State/Provinces/Countries page in the NetSuite user interface (see figure).

-   Go to _Setup > Company > States/Provinces/Counties_.
    

Note that some short name values may contain characters that are not translated in some languages. You can retrieve a list of translated short names through SOAP web services. However, in SOAP web services, you cannot use the search operation to retrieve state values. You must use the **getAll** operation to retrieve all state values in the system. This operation will return **all** states, not the legal ones for your default country. Also note that the country and state must match on the address.

Be aware that state values can be added, updated, and deleted through the NetSuite user interface and through SOAP web services. For information about working with states, provinces, and counties in the user interface, see [Setting Up States, Provinces, and Counties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N253697.html).

State and province names in SOAP web services must match the short name values listed at _Setup > Company > States/Provinces/Counties_.

The Java and SOAP samples below show how to create a new customer and define all address properties on the customer Address (addressbook) sublist. Note that the state value is defined as the string **"** CA **"** - as it appears on the States/Provinces/Counties page in the UI.

## Java {#bridgehead_N3796270}

          `public void add_customer_with_address() throws Exception { Customer c = new Customer(); c.setCompanyName("my company"); CustomerAddressbook cab = new CustomerAddressbook(); cab.setAddr1("123 Main St"); cab.setCity("San Mateo"); cab.setState("CA"); cab.setZip("94403"); cab.setCountry(Country._unitedStates); c.setAddressbookList(new CustomerAddressbookList(new     CustomerAddressbook[]{cab}, false)); sessMgr.getPort().add(c); }` 
        

## SOAP {#bridgehead_N3796280}

          `<add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <record externalId="Strawberry10150306" xsi:type="ns1:Customer"       xmlns:ns1="urn:relationships_2017_1.lists.webservices.netsuite.com">                <ns1:companyName xsi:type="xsd:string">my company</ns1:companyName>                <ns1:addressbookList replaceAll="false" xsi:type="ns1:CustomerAddressbookList">                   <ns1:addressbook xsi:type="ns1:CustomerAddressbook">                      <ns1:addr1 xsi:type="xsd:string">123 Main St</ns1:addr1>                      <ns1:city xsi:type="xsd:string">San Mateo</ns1:city>                      <ns1:zip xsi:type="xsd:string">94403</ns1:zip>                      <ns1:country xsi:type="ns2:Country"          xmlns:ns2="urn:types.common_2017_1.platform.             webservices.netsuite.com">_unitedStates          <ns1:country>                      <ns1:state xsi:type="xsd:string">CA</ns1:state>                   </ns1:addressbook>                </ns1:addressbookList>             </record>          </add>` 
        

## Creating Custom State Values {#bridgehead_N3796318}

For countries that do not have country/state values built in to NetSuite (for example, Portugal or Argentina), you can create a list of custom state values and assign these values to a specific country. Doing so enables you to enforce country/state validation when the _Allow Free-Form States in Addresses_ is set to FALSE.

Note:

See [Setting the Allow Free-Form States in Addresses Preference](#bridgehead_N3796390) for more information about setting this preference and enabling or disabling country/state validation.

Create custom state values by going to _Setup > Company > States/Provinces/Counties > New_. In the Country dropdown list, select your country. In the Full Name and Short Name fields, specify your state values. Note that you must use the **Short Name** value in your SOAP web services requests.

Note:

You can also click the New button at the top of the State/Province/Countries list page to create custom states.

## Setting the Allow Free-Form States in Addresses Preference {#bridgehead_N3796390}

Selecting the **Allow Free-Form States in Addresses** preference controls whether country/state validation is performed during a SOAP web services request. In the user interface, go to _Setup > Company > General Preferences_.

Important:

If you enable this preference, you must enter the two-letter abbreviation for the state or province for the system to properly determine the transaction nexus. If you use the full name of the state or province, the system will not be able to determine the correct transaction nexus.

#### To enable country/state validation: {#procedure_N3796409}

1.  Make sure the **Allow Free-Form States in Addresses** box is not checked. When the box is not checked, the system validates the state short name (for example, CA or GA) against the country.
    
2.  In your SOAP web services request, you must then submit the abbreviation that exists in the _Setup > Company > States/Provinces/Counties_ list, in the **Short Name** column.
    
3.  If the country/state values do not exist in the user interface, extend this list by going to _Setup > Company > State/Provinces/Countries > New_ to define custom states and associate them with a country. (See [Creating Custom State Values](#bridgehead_N3796318) for more information about creating custom state values.)
    

#### To disable country/state validation: {#procedure_N3796462}

1.  Make sure the **Allow Free-Form States in Addresses** box is checked
    
2.  In your SOAP web services request, send any state value in the request. NetSuite stores the value you send as a string.
    

### Related Topics

-   [Country, State, and Language Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3784994.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
