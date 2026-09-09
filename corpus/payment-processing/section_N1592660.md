---
id: "section_N1592660"
type: "section"
title: "Setting Up Payment Aggregation Methods"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Setting Up Electronic Bank Payments > Setting Up Payment Aggregation Methods"
parent: "section_3831186542"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1592660.html"
anchors: ["procedure_N1592679"]
sha256: "f6b8938ec24688323b33c8de442479728da0e056766133bc3abf20a6976c4509"
---

Aggregation defines the way bills and expenses are grouped together to create a payment record. Using payment aggregation, a payment record is created for multiple bills grouped according to the aggregation method specified.

By default, payment aggregation is done per payee (vendor or employee). For example, when you check the payment aggregation box on the EFT - Bill Payments form without selecting a payment aggregation method, payment records are created for each vendor or employee included in the Select Transactions sublist.

If you check the payment aggregation box and select a specific payment aggregation method, payments are grouped based on the method within each vendor or employee. For example, if you created a custom field called Purchase Contract and tagged each invoice to a specific Purchase Contract value, the payments are grouped based on this field value.

Payment Aggregation doesn't affect the **Status Summary** field of a Payment File Administration (PFA) record. The value of this field is based on the total number of transactions marked and paid when processing the PFA record.

Note:

The maximum number of transactions to be processed for payment per batch, is 5000 or less, depending on the custom template setup. Regardless of whether payment transactions to be created during processing are aggregated or not, you cannot exceed the maximum number of transactions.

#### To set up payment aggregation methods: {#procedure_N1592679}

1.  Go to Payments > Setup > Payment Aggregation > New.
    
2.  In the **Name** field, enter a name for this payment aggregation method.
    
3.  In the **Transaction Field ID** field, enter the internal ID of the field that you want use as the basis for the aggregation method. The fields that can be used for aggregation are found on the vendor bill and expense report forms.
    
    For example, if you want to aggregate payments by due date, enter the internal ID of the **Due Date** field:
    
    **duedate**
    
    Note:
    
    For aggregation method, you can only use a field that's available for all four types of entities (employee, customer, vendor, or partner); otherwise, an error will be generated because the aggregation method is invalid.
    
    For information about locating internal IDs of fields, see [Finding Internal IDs of Record Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0416043804.html)
    
4.  Check the **Inactive** box to make this payment aggregation method inactive.
    

### Related Topics

-   [File Cabinet Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N541319.html)
-   [Setting Up Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3831186542.html)
-   [Setting Up Payments Tab Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1589991.html)
-   [Creating Folders in the NetSuite File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1590174.html)
-   [Setting Up Bank Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1590309.html)
-   [Adding the Payment Batch Processing Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1666182.html)
-   [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
