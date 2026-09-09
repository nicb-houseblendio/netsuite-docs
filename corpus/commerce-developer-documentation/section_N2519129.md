---
id: "section_N2519129"
type: "section"
title: "customer"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Commerce API > JSON Object Fields > customer"
parent: "section_N2512816"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2519129.html"
anchors: []
sha256: "b50ec51afc953eaef9b0664d125c1d3529a4699bf5a9369ee5ee8559b2c9b798"
---

This object contains information about the logged in customer.

| Field Name | Field Type | Description | In Get Functions? | In Set Functions? |
| --- | --- | --- | --- | --- |
| addressbook | List of JSON [address](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2514053.html) objects | Address information | yes | no |
| balance | string | Customer's accounts receivable balance due, shown in customer's currency. | yes | no |
| campaignsubscriptions | List of JSON subscription objects | Information about campaign subscriptions for the given customer. | yes | yes |
| companyname | string | Customer company name | 
yes

(for Checkout and Shopping domains)



 | yes (for Checkout domain only) |
| cookieoptions | boolean | Returns a list of cookies for which the customer selected to opt in or out. These are returned only when the SuiteCommerce Analytics Data feature is enabled. For example: "cookieoptions": {"ANALYTICS": false, "PERFORMANCE": true} | yes | yes |
| creditcards | List of JSON [creditcard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2518010.html) objects | Credit card information | yes | no |
| creditholdoverride | string | Customer's credit hold status. | yes | no |
| creditlimit | string | Maximum currency amount the customer is allowed to accrue in outstanding receivables. | yes | no |
| email | string | Customer email address Required in Set function for customer registration, guest registration, and login. | no | yes |
| emailsubscribe | string | Email subscription Value should be T or F. | yes | yes |
| firstname | string | Customer first name | yes | yes |
| internalid | string | Internal ID | yes | no |
| isperson | boolean | If false this customer is of customer type. If true this customer is of the type individual. | yes | no |
| lastname | string | Customer last name | yes | yes |
| middlename | string | Customer middle name | yes | yes |
| name | string | Customer name Important: As of Version 2013 Release 1, this field is no longer used and is included for backward compatibility only. The firstname, lastname, and middlename fields are the preferred fields for getting and setting customer names. | yes | yes |
| partner | string | Partner | yes | yes |
| password | string | Password Required in Set function for customer registration and login. | no | yes |
| password hint | string | Hint | no | yes |
| paymentterms | JSON object of fields | Payment terms associated with the customer. These are returned only if the website sales order type is set to Per Customer Basis. | yes | no |
| phoneinfo | JSONobject of fields | 

Returns or sets the phone number information for a customer.

For example: {"phone":"65460780", "fax" : "40540", "altphone" : null}



 | yes | yes |

### Related Topics:

-   [ShoppingSession Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2497708.html)
-   [Customer Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2503226.html)
-   [Order Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2506263.html)
-   [PageGenerator Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2510548.html)
-   [StandardTagLibrary Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2511297.html)
-   [Shopping Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496577.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
