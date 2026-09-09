---
id: "procedure_N1321905"
type: "procedure"
title: "Contract Items Creation"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Software Vertical Contract Renewals > Setting Up Contract Renewals > Setting Up Contract Renewals Preferences > Contract Items Creation"
parent: "section_N1321619"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/procedure_N1321905.html"
anchors: []
sha256: "9cbbbfbaa78dcaf3ddc4aff1d53993c17394dcbfc676301d18773935111a69d4"
---

These preferences affect how contract items are generated:

| Field | Description |
| --- | --- |
| Enable Script R03 | Check this box to enable the script that creates contract items. Note: The R03 script doesn't support multiple queues. To prevent unexpected behavior, make sure that all R03 deployments are assigned to the same queue. |
| Search: CI Pending Creation | If you want to use a saved search to define the list of transactions that will be processed by the R03 script for contract item creation, check the **Use CI Pending Creation Search** box and specify the saved search that you want to use in this field. The list returned by the saved search will be further filtered by the status selected in the **Transaction Status to Process** preference. Note: To avoid any errors, don't select the default search (**Contract Item Pending Creation**) in this field if the **Use CI Pending Creation Search** box is checked. For information about creating a custom saved search for contract item creation, see [Using a Custom Saved Search for Contract Item Creation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162002114965.html). |
| Transaction Status to Process | Select which transactions status will be processed to create contract items. |
| Item Category to Process | Select the item categories that generate contract items. Note: For service items, select **Service - Perpetual** to generate perpetually-licensed service items that have no expiration date and no renewal action is required or select **Services** to generate term-licensed service items. |
| Require License for M/S Items (Renewal) | Check this box if you want the contract item creation script (R03) to require product license items in transactions. Clear this box if you want to enable creation of contracts from transactions with no product license. |
| Use CI Pending Creation Search | Check this box if you want to use a saved search to define the list of transactions that will be processed by the R03 script for contract item creation. You can specify the saved search that you want to use in the **Search: CI Pending Creation** field. For information about creating a custom saved search for contract item creation, see [Using a Custom Saved Search for Contract Item Creation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162002114965.html). If this box is cleared, R03 will use its default search to filter transactions that will be processed for contract item creation. Note: Regardless if this box is checked or cleared, the transactions to be processed by R03 will be filtered based on the status selected in the **Transaction Status to Process** field. |

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
