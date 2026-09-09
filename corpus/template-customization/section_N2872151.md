---
id: "section_N2872151"
type: "section"
title: "Using a Standard #10 Window Envelope With Transactions"
branch: "template-customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Template Customization > Basic Printing Layouts > Customizing Transaction Form PDF Layouts > Using a Standard #10 Window Envelope With Transactions"
parent: "section_N2869660"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2872151.html"
anchors: ["procedure_N2872162"]
sha256: "ad2f6fe1c5129426eb1d3e9c371cfd8f9f87ab6570588cc7738b9dfbdf4e1d79"
---

If you use window envelopes, you may need to adjust the printing position of your PDF transaction forms to show the correct address through the window.

If your account is set up to use metric measurement, convert the imperial values provided in the following procedure.

#### To adjust your standard layouts to fit in a standard #10 window envelope: {#procedure_N2872162}

1.  Go to _Customization > Forms > Transaction Form PDF Layouts_ (or Transaction Form HTML Layouts).
    
2.  Click **Customize** next to the layout you want to change.
    
3.  In the **Name** field, enter a name for your custom layout.
    
4.  Click the **Elements** subtab.
    
5.  Click **Border & Placement**.
    
6.  In the **Border & Placement** section, locate the **Bill To** row.
    
7.  In the **Left** column, enter **1**.
    
    This moves the left edge of the field 1 inch from the left margin of the page.
    
8.  In the **Top** column, enter **2.25**.
    
    This moves the top edge of the field 2.25 inches from the top margin of the page.
    
9.  In the **Right** column, enter **4.2**.
    
    This moves the right edge of the field 4.2 inches from the left margin.
    
10.  In the **Bottom** column, enter **3.5**.
     
     This moves the bottom edge of the field 3.5 inches from the top of the page.
     
11.  Locate the **Ship To** row.
     
12.  In the **Left** field, enter **4.55**.
     
     This moves the left edge of the field 4.55 inches from the left margin of the page.
     
13.  In the **Top** column, enter **2.25**.
     
     This moves the top edge of the field 2.25 inches from the top margin of the page.
     
14.  In the **Right** column, enter **8**.
     
     This moves the right edge of the field 8 inches from the left margin.
     
15.  In the **Bottom** column, enter **3.5**.
     
     This moves the bottom edge of the field 3.5 inches from the top of the page.
     
16.  When you've finished, click **Submit**.
     
     You're returned to the Custom Layouts list.
     
17.  Check the box in the **Preferred** column next to your custom layout.
     
     This ensures that your layout is applied to all forms of that type.
     
18.  Click **Save**.
     

To adjust any transaction form layouts that you want to mail in standard #10 window envelopes, repeat the preceding steps. You can adjust any of your transaction form layouts for any size window envelope. Measure your envelope and the placement of the window to determine where to place the address.

When you have the measurements for your envelope and determined where to place the address field, you need to convert the fraction measurements into decimal measurements to adjust the layout. Use the following table as a quick reference guide to convert fraction measurements into decimal measurements.

| **Fraction** | **Decimal** | **Fraction** | **Decimal** |
| --- | --- | --- | --- |
| 1/2 | 0.5 | 1/16 | 0.0625 |
| 1/4 | 0.25 | 3/16 | 0.1875 |
| 1/3 | 0.33 | 5/16 | 0.3125 |
| 3/4 | 0.75 | 7/16 | 0.4375 |
| 2/3 | 0.67 | 9/16 | 0.5625 |
| 1/8 | 0.125 | 11/16 | 0.6875 |
| 3/8 | 0.375 | 13/16 | 0.8125 |
| 5/8 | 0.625 | 15/16 | 0.9375 |
| 7/8 | 0.875 | \- | \- |

### Related Topics

-   [Customizing Transaction Form PDF Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2869660.html)
-   [Defining Custom Elements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2871444.html)
-   [Configuring Borders and Placement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2870073.html)
-   [Formatting Label Text](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2870892.html)
-   [Formatting Data Text](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2871160.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
