---
id: "section_N1796409"
type: "section"
title: "Setting Up Tax Agencies as Vendors"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Enabling and Setting Up Taxation Features > Setting Up Tax Agencies as Vendors"
parent: "chapter_N1794679"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1796409.html"
anchors: ["procedure_N1796465"]
sha256: "d8f3f4498c0e9edab2ee7e3397c2e73fd18f6a6d38b02e487d5d825abd29fe2e"
---

In most countries, businesses are required to collect tax from sales. Then, the collected tax must be paid to the tax authority on behalf of the customers. Default tax agencies are automatically set up by the system when you create a subsidiary or nexus, but you must edit the tax agency vendor record to provide details such as address information.

In a OneWorld account, multiple subsidiaries can pay taxes to the same tax agency. When you add a subsidiary, and its nexus is the same as that of an existing subsidiary, NetSuite creates a copy of the preferred tax vendor for that nexus to associate it with the new subsidiary. This copy (known as a child or shadow vendor) is necessary because tax agency vendors can't be shared between subsidiaries. However, you can share non tax agency vendors with multiple subsidiaries. For more information, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).

Note:

The child tax vendors that NetSuite creates when subsidiaries share a tax nexus are hidden, and therefore can't be used directly in transactions.

Accounts associated with tax agency vendors are tax control accounts. If you want to attach an A/P account to a vendor, make sure the vendor type isn't tax agency.

If you use tax codes in transactions, NetSuite posts tax to the appropriate tax agency associated with the subsidiary.

Don't use Write Check to pay a tax agency. If you want to pay liabilities to a tax agency, you must go to _Transactions > Bank > Write Tax Liability_ , where you can select the appropriate tax agency in the **Payee** field.

An administrator can create a vendor record for a tax agency if necessary.

#### To set up a tax agency as a vendor: {#procedure_N1796465}

1.  Go to _Lists > Relationships > Vendors > New_
    
2.  On the Vendor page, specify the governmental authority to which you must pay tax. For example, in the **Vendor** field, you can enter the name of the state or provincial tax agency where your business is located.
    
3.  In the **Category** field on the **Info** subtab, be sure to select **Tax Agency**.
    
4.  Enter any additional information as needed.
    
5.  Click **Save**.
    

You can select this tax agency when you set up tax preferences and tax codes.

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html)
-   [Tax Code Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805973.html)
-   [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html)
-   [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html)
-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Paying Sales Tax - United States](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2041996.html)
-   [Paying Provincial Sales Tax - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1859840.html)
-   [Paying Tax Liabilities - Non-U.S. Editions and Nexuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1817593.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
