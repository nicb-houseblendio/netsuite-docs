---
id: "bridgehead_N2139089"
type: "bridgehead"
title: "Sum of Years' Digits Depreciation Method"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Setting Up the Fixed Assets Management System > Depreciation Methods > Preconfigured Depreciation Methods > Sum of Years' Digits Depreciation Method"
parent: "section_N2137654"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2139089.html"
anchors: []
sha256: "9c561c7ab46ad45493044eb765caad6a5b19e7f46beababadcd343fa48dbea03"
---

Sum-of-Years' Digits is a depreciation method that results in a more accelerated write-off than straight line, but less than declining-balance method. With this method, annual depreciation is determined by multiplying the depreciable cost by a set of fractions.

-   **Depreciable Cost = Original Cost - Salvage Value**
    
-   **Book Value = Original Cost - Accumulated Depreciation**
    

Example: If an asset has original cost $1,000, a useful life of five years and a salvage value of $100, to calculate its depreciation schedule:

1.  Determine Years' digits. Because the asset has a useful life of five years, the Years' digits are: 5, 4, 3, 2, and 1.
    
2.  Calculate the sum of the digits. 5+4+3+2+1=15
    
    Depreciation rates are as follows:
    
    -   5/15 for the 1st year
        
    -   4/15 for the 2nd year
        
    -   3/15 for the 3rd year
        
    -   2/15 for the 4th year
        
    -   1/15 for the 5th year
        

| **Book Value - Beg. of Year** | **Total Depreciable Cost** | **Depreciation Rate** | **Depreciation Expense** | **Accumulated Depreciation** | **Book Value - End of Year** |
| --- | --- | --- | --- | --- | --- |
| $1,000 (Original Cost) | $900 | 5/15 | $300 ($900 \* 5/15) | $300 | $700 |
| $700 | $900 | 4/15 | $240 ($900 \* 4/15) | $540 | $460 |
| $460 | $900 | 3/15 | $180 ($900 \* 3/15) | $720 | $280 |
| $280 | $900 | 2/15 | $120 ($900 \* 2/15) | $840 | $160 |
| $160 | $900 | 1/15 | $60 ($900 \* 1/15) | $900 | $100 (Scrap Value) |

### Related Topics

-   [Preconfigured Depreciation Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2137654.html)
-   [Nordic Countries and Benelux Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1118074836.html)
-   [Japan Depreciation Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1118074915.html)
-   [Asset Usage (Asset Activity) Depreciation Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2137764.html)
-   [Fixed Declining (Declining Balance) Depreciation Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2138448.html)
-   [Straight Line Depreciation Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2138790.html)
-   [Straight Line Remaining Depreciation Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2139576.html)
-   [Sum of Years/Straight Line Depreciation Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2139588.html)
-   [150DB and 200DB Depreciation Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2139600.html)
-   [4-4-5 Calendar Depreciation Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4302913229.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
