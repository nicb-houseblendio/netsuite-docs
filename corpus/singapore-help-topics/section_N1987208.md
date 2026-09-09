---
id: "section_N1987208"
type: "section"
title: "Accounting for Goods and Services Tax - Singapore"
branch: "singapore-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Singapore Help Topics > Singapore Tax Topics for Accounts Without SuiteTax > Accounting for Goods and Services Tax - Singapore"
parent: "chapter_N1981261"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1987208.html"
anchors: ["procedure_N1987224"]
sha256: "35dbb64f363e688a06e2aa4750b167f3e4431df070271b24c5e3df5f5c8998b0"
---

GST is a broad-based consumption tax levied on the import of goods (collected by Singapore Customs), as well as nearly all supplies of goods and services in Singapore. The only exemptions are for the sales and leases of residential properties and the provision of most financial services. Export of goods and international services are zero-rated. In other countries, GST is known as Value Added Tax (VAT).

GST is computed by computing the output tax from sale transactions less the input tax from purchase transactions. In NetSuite, input tax is applied by default to a GST asset account, and output GST is applied in turn to a liability account. At the end of a tax period, you make a journal entry to account for the final VAT in the appropriate liability account so you can pay your VAT tax liability.

#### To post net VAT (output tax less input tax) to the GST Liability account: {#procedure_N1987224}

1.  Go to _Transactions > Financial > Make Journal Entries_.
    
    1.  Select the posting period for this journal.
        
    2.  Pick or enter a date for the journal entry.
        
    3.  In the **Account** field, select **GST on Purchases**.
        
    4.  In the **Credit** column, enter the amount you want to apply to the GST Liability account.
        
2.  Click **Add**.
    
3.  In the **Account** column, select **GST Liability**. The amount you entered on the previous line automatically fills in the **Debit** column.
    
4.  Click **Add**
    
5.  Click **Save**.
    
6.  Go to _Transactions > Financial > Make Journal Entries_.
    
    1.  Select the posting period for this journal.
        
    2.  Pick or enter a date for the journal entry.
        
    3.  In the **Account** field, select **GST Liability**.
        
    4.  In the **Credit** column, enter the amount you want to apply to the GST Liability account.
        
7.  Click **Add**.
    
8.  In the **Account** column, select **GST on Sales**. The amount you entered on the previous line automatically fills in the Debit column.
    
9.  Click **Add**.
    
10.  Click **Save**.
     

Now, you can pay your tax liability. For more information, read [Paying Tax Liabilities - Non-U.S. Editions and Nexuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1817593.html).

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Additional Setup Requirements for Singapore](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1981722.html)
-   [Setting Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1813668.html)
-   [Setting Tax Rounding Levels, Methods, and Precision Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1814149.html)
-   [Singapore Tax Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983547.html)
-   [Singapore Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1983994.html)
-   [Singapore GST Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1987604.html)
-   [Singapore Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1989169.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
