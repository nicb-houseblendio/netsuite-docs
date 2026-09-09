---
id: "section_N2365187"
type: "section"
title: "Creating a Tax Agency Vendor Record"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Records > Vendor Record Management > Creating a Tax Agency Vendor Record"
parent: "article_161951406143"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2365187.html"
anchors: ["procedure_N2365211"]
sha256: "62c876c48f1c7f7ff07828f4f4c2b466e669633210e9071c314d1ad050e0c3b6"
---

In most locations, you are required by government to collect tax from your customers when you sell merchandise. Then, you pay that tax on their behalf to the taxing authority. In NetSuite, you can set up sales tax items and sales tax vendors to simplify the sales tax collection and payment process.

In a NetSuite OneWorld account, multiple subsidiaries can pay taxes to the same tax agency. Tax agency vendors can"t be shared between subsidiaries. Therefore, NetSuite creates a copy (child or shadow vendor) of the preferred tax vendor for that nexus to associate it with a new subsidiary. The child tax vendors that NetSuite creates when subsidiaries share a tax nexus are hidden and therefore can"t be used directly in transactions. You can, however, share non tax agency vendors with multiple subsidiaries.

For more information, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).

#### To create a tax agency vendor record: {#procedure_N2365211}

1.  Go to _Lists > Relationships > Vendors > New_.
    
2.  On the Vendor page, create a record for the governmental authority to which you pay sales tax.
    
    For example, in the **Vendor ID** field, you can enter the Secretary of State where your business is located.
    
3.  In the **Category** field, under Primary Information, be sure to select **Tax Agency**.
    
4.  Enter any additional information.
    
5.  When you have finished, click **Save**.
    

After this vendor is set up, you can create tax codes that you associate with the sales tax vendor. Go to _Setup > Accounting > Taxes > Tax Codes > New_.

You must identify a vendor as a tax agency to ensure that it appears as such in accounting lists. For example, you want to display Tax Agency next to a vendor's name on the Vendors list page. Go to _Setup > Accounting > Accounting Lists > Vendor Category_, and then check the Tax Agency box.

As you create invoices and cash sales receipts, NetSuite sums the tax for each transaction. It shows it on the invoice or receipt as a line item.

As sales tax becomes due, you can pay it by going to the Sales Tax Payment page. Go to _Transactions > Bank > Pay Sales Tax_.

### Related Topics

-   [Vendor Record Configuration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161952107343.html)
-   [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html)
-   [Editing a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4443197067.html)
-   [Inactivating Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4443201053.html)
-   [Deleting a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4443213535.html)
-   [Merging Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4443233738.html)
-   [Vendor Dashboards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4849482517.html)
-   [Printing Mailing Labels for Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2368875.html)
-   [Vendor Record Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161951406143.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
