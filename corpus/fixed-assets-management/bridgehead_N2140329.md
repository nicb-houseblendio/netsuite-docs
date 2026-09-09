---
id: "bridgehead_N2140329"
type: "bridgehead"
title: "Formula Example: Maximum of Two Values"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Setting Up the Fixed Assets Management System > Depreciation Methods > Depreciation Formula > Formula Example: Maximum of Two Values"
parent: "section_N2140095"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2140329.html"
anchors: []
sha256: "15275099ea0fb592a9803113ed625378c20e3e3a319f0fd59200dbfefc228f83"
---

The formula can perform two separate depreciation calculations, and then apply the one that results in the higher depreciation amount. To use this functionality, separate the two formulas by the ~ character.

For example, the formula for the 150DB method is:

((NB-RV)\*(1.5/AL))~((NB-RV)/(AL-CP+1))

Fixed Assets Management calculates the results of both expressions individually and then uses the higher amount for the depreciation. In this case, the first formula returns the highest value for the first part of the asset's life before switching to the second.

Month 1

Net book value: 20,000

Residual value: 2,000

Asset lifetime: 60 (5 years)

Current period: 1

((20,000 - 2,000)\*(1.5/60)) = 450

((20,000 - 2,000)/(60 - 1 + 1)) = 300

Therefore the first formula (450) is used.

Month 30

Net book value: 10,409

Residual value: 2,000

Asset lifetime: 60 (5 years)

Current period: 30

((10,409 - 2,000)\*(1.5/60)) = 210

((10,409 - 2,000)/(60 - 30 + 1)) = 271

Now the second formula (271) is used, and that same amount applies for the rest of the asset's life because the second is a straight line depreciation method. In this example, the formula switches a third of the way through, around period 20.

### Related Topics

-   [Depreciation Formula](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2140095.html)
-   [Formula Example: Straight Line Depreciation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2140285.html)
-   [Formula Example: Diminishing Value Method for Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2140427.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
