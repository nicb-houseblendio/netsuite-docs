---
id: "section_N1243551"
type: "section"
title: "Show the Customer Account Balance Due on Invoices"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Invoices > Show the Customer Account Balance Due on Invoices"
parent: "section_N1235134"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1243551.html"
anchors: ["procedure_N1243569"]
sha256: "529ce81195313794026681339dabc456e65ae0723356e970eb2cd797ef7c95b4"
---

You can inform customers of the outstanding balance due on their account by showing their total account balance on each invoice. This is a good way to keep customers aware of their balance due between statements.

The balance on an invoice is the customer's total amount due on their account, including the amount of the invoice it's printed on.

To show the customer account balance on invoices, you need to customize your standard invoice form. Then, you can select this custom form when creating an invoice.

#### To customize an invoice to show the Balance field: {#procedure_N1243569}

1.  Go to _Customization > Forms > Transaction Forms_ (Administrator).
    
2.  Next to the invoice form to which you want to add the **Balance** field, click **Customize**.
    
    In the **Name** field, enter a name for this form. For example, **Balance Field Invoice**.
    
3.  Click the **Screen Fields** subtab.
    
    On the **Billing** subtab, check the box in the **Show** column next to Balance.
    
    If you use the Consolidated Payments feature, check the **Consolidated Balance** box to show the consolidated balance.
    
4.  Click the **Printing Fields** subtab.
    
5.  Click the **Body** subtab.
    
6.  Check the box in the **Print/Email** column next to Balance.
    
    If you use the Consolidated Payments feature, check the **Consolidated Balance** box to show the consolidated balance.
    
7.  If you want this to be the preferred form, check the **Form is Preferred** box in the header.
    
8.  Click **Save**.
    

Now, when you create invoices using this form, the customer's account balance shows in the **Balance** field. This balance shows on the invoice when it's viewed, printed, faxed or emailed.

Note:

When you view an old invoice, you'll see the balance due at the time the invoice was created. To update the balance, edit the invoice.

### Related Topics

-   [Custom Workflow Based Invoice Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1235332.html)
-   [Global Invoicing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1237960.html)
-   [Creating an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1238506.html)
-   [Choosing an Invoice Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240040.html)
-   [Billing or Invoicing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240951.html)
-   [Closing or Voiding an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158654862294.html)
-   [Invoicing Billable Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1241287.html)
-   [Creating Installments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540928779.html)
-   [Printing an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1242104.html)
-   [Progress Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1243687.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
