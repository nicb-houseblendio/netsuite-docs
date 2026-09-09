---
id: "section_N2623719"
type: "section"
title: "Customer Attributes"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Creating Attribute Tags > Creating Attribute Tags for Standard Records > Customer Attributes"
parent: "section_N2616966"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2623719.html"
anchors: []
sha256: "c4bf5f4bdb87be525268d7548f771fc766c87c50f526f09d4525391156732e00"
---

The following table includes the eligible fields for the customer record type and the corresponding attribute to use in your tag. Attributes are not case-sensitive. For example, you could use the Attribute tag below to display the customer price level on your site:

          `<%=getCurrentAttribute('customer','pricelevel')%>` 
        

| **Field Name** | **Attribute** | Notes |
| --- | --- | --- |
| Inactive | isinactive |  |
| Internal ID | internalid |  |
| Price Level | pricelevel pricelevel1, pricelevel2, etc. | Use **pricelevel** to return the price for the customer who is logged in. Use **pricelevel** followed by a numeric value, representing the price level ID, to return other price levels on the item record. Use the Price level List at Setup > Accounting > Accounting Lists to determine the correct ID. |
| Subsidiary | subsidiary |  |
| Account | accountnumber |  |
| Address | defaultaddress |  |
| Alternate Name | altname | This attribute returns the Company Name for companies, for individuals, it returns the First and Last name. Note: You must have the proper setup for Auto Generated numbers to use the attribute tag for alternative name. Go to Setup > Company > Auto Generated number. On the Entities subtab, check the **Allow Override** box for Customer records. |
| Alt. Email | altemail |  |
| Alt. Phone | altphone |  |
| Balance | balance |  |
| Campaign Category | campaigncategory |  |
| Category | category |  |
| Child Of | parent |  |
| Comments | comments |  |
| Company Name | companyname |  |
| Credit Limit | creditlimit |  |
| Currency | currency |  |
| Customer ID | entityid |  |
| Date Created | datecreated |  |
| Days | daysoverdue | This attribute displays the days overdue on the balance. |
| Email | email |  |
| Email Preference | emailpreference |  |
| End Date | enddate |  |
| Fax | Fax |  |
| Give Access | giveaccess |  |
| Home Phone | homephone |  |
| Image | imagehtml |  |
| Project Title | title |  |
| Language | language |  |
| Lead Source | leadsource |  |
| Mobile Phone | mobilephone |  |
| Mr./Ms. | salutation |  |
| Name | firstname | This attribute returns the first name for individuals. |
| Other Relationships | otherrelationships |  |
| Overdue (balance) | overduebalance |  |
| Partner | partner |  |
| Phone | phone |  |
| Pref. CC Processor | prefccprocessor |  |
| Reminder Days | reminderdays |  |
| Resale Number | resalenumber |  |
| Role | accessrole |  |
| Sales Rep | salesrep |  |
| Ship Complete | shipcomplete |  |
| Shipping Item | shippingitem |  |
| Start Date | startdate |  |
| Status | entitystatus |  |
| Taxable | taxable |  |
| Tax Item | taxitem |  |
| Tax Reg. Number | vatregnumber |  |
| Terms | terms |  |
| Territory | territory |  |
| Unsubscribe | unsubscribe |  |
| Address | url |  |

### Related Topics

-   [Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2617271.html)
-   [Information Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2620223.html)
-   [Color Theme Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622110.html)
-   [Category Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622893.html)
-   [Site Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2625840.html)
-   [Request Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627019.html)
-   [Checkout Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627341.html)
-   [Order Confirmation Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627572.html)
-   [Creating Attribute Tags for Standard Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
