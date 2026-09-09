---
id: "section_N1302583"
type: "section"
title: "Sending Individual Collection Letters"
branch: "overdue-balances-and-collections"
category: "order-management"
breadcrumb: "Order Management > Overdue Balances and Collections > Collections > Sending Individual Collection Letters"
parent: "chapter_4418080075"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1302583.html"
anchors: ["procedure_N1302665"]
sha256: "48f37fbe16eb695eb2e41ec5dc3bb7de4450f34e4b568e79c1cb0ea04e51bf7f"
---

You can also choose to send out individual collection letters with details of an overdue invoice.

First, you create and upload the template you want to use for the collection letter. For more information, see [Working with Email Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N514744.html).

You can include transaction CRMSDK tags in the text of your template that refer to specific fields in the transaction. For collection letters, the following CRMSDK tags might be useful:

-   **NLTRANID** - replaced with the transaction number
    
-   **NLTRANDATE** - replaced with the transaction date
    
-   **NLTOTAL** - replaced with the total
    

For a complete list of CRMSDK tags that reference transactions, see [CRMSDK Tags for Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N515605.html#bridgehead_N521522).

Next, navigate to the overdue invoice to send the message.

#### To send an individual collection letter: {#procedure_N1302665}

1.  View the overdue invoice.
    
2.  Click the **Communication** subtab.
    
3.  Click the button for the type of message you want to send.
    
4.  In the message window, click the **Message** subtab.
    
5.  Select the collections letter template in the **Template** field.
    
6.  Click **Merge & Send**.
    

This message is saved on the Messages subtab of the invoice, giving you a record of the communication.

### Related Topics:

-   [Sending Collection Letters in Bulk](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1302167.html)
-   [Viewing Overdue Balances on the Customer Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1302769.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
