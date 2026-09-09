---
id: "section_N2393276"
type: "section"
title: "Applying a Vendor Credit"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Credits > Applying a Vendor Credit"
parent: "chapter_N2391960"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2393276.html"
anchors: ["procedure_N2393303", "procedure_N2393393", "procedure_N2393454"]
sha256: "a66d90facf1aafa29afc0fadc46bedd990c99817acd40d41c00c2ece16aacd9c"
---

You can apply vendor credits to decrease the amount owed to a vendor. When you apply a vendor credit against an open bill, the amount of the credit is deducted from the total amount of the bill.

You can apply a vendor credit to a bill on the credit transaction or on a payment transaction. You can also apply part of a vendor credit.

#### To apply vendor credit on the credit transaction: {#procedure_N2393303}

1.  Go to _Transactions > Payables > Enter Vendor Credits > List_.
    
2.  On the **Bill Credits** page, click **Edit** next to the credit you want to apply.
    
3.  In the **Items** subtab on the **Bill Credit** page:
    
    -   Check the **Auto-Apply** box if you want NetSuite to apply the credit amount to the oldest vendor bills due.
        
    -   Click the **Apply** subtab to apply the credit toward a specific vendor bill.
        
    -   Check the **Apply** box next to the bills you want the credit applied to.
        
4.  Click **Save**.
    

Now, when you include the bill you credited on a payment, your payment amount reflects the vendor credit.

You can also apply vendor credits when you enter a payment transaction.

#### To apply credit on a bill payment: {#procedure_N2393393}

1.  Go to _Transactions > Payables > Pay Bills_.
    
2.  On the **Bill Payment** page, check the **Pay** box next to each bill you want to pay and each credit you want to apply.
    
    You must have open bills from the vendor to apply a credit from that vendor.
    
3.  Click **Save**.
    

The vendor credit is applied to the bills for that vendor, and the credit amount is deducted from the total amount paid to the vendor.

#### To apply credit on a single vendor payment: {#procedure_N2393454}

1.  Go to _Transactions > Purchases/Vendors > Pay Single Vendor_.
    
2.  On the **Bill Payment** page, select the vendor you want to pay.
    
    Open bills and credits for that vendor appear.
    
3.  Check the **Apply** box next to each bill you want to pay and each credit you want to apply.
    
    You must have open bills from the vendor to apply a credit from that vendor.
    
4.  Click **Save**.
    

The vendor credit is applied to the bills for that vendor, and the credit amount is deducted from the total amount paid to the vendor.

After you have applied a vendor credit, you can review how it was applied in the following ways:

-   **On a Payment**:
    
    1.  Go to _Transactions > Payables > Pay Bills_.
        
    2.  On the **Bill Payments** page, next to the payment, click **View**.
        
        The **Credits Applied** subtab shows which credits were applied.
        

-   **On a Credit**:
    
    1.  Go to _Transactions > Payables > Enter Vendor Credits > List_.
        
    2.  On the **Bill Credits** page, next to the credit, click **View**.
        
    3.  The **Apply** subtab shows which bills were credited.
        

If you void a bill payment, the credits previously applied no longer show on that payment.

Important:

After you have applied credit to a bill, deleting the bill payment doesn't automatically unapply credits that were applied to it. You must unapply the vendor credits separately.

### Related Topics

-   [Entering Vendor Credits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2392083.html)
-   [Entering a Vendor Credit Manually](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1493669913.html)
-   [Creating a Vendor Credit Directly From a Vendor Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2392547.html)
-   [Associating a Vendor Credit With a Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2392806.html)
-   [Creating a Vendor Credit Directly From a Vendor Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2393090.html)
-   [Viewing Vendor Credits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162341387037.html)
-   [Removing Credits From Deleted Vendor Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2393719.html)
-   [Vendor Credit Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161107139523.html)
-   [Vendor Credits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2391960.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
