---
id: "bridgehead_N1123880"
type: "bridgehead"
title: "Determine Commission Categorization and Eligibility"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Commissions > Employee Commission Schedules > Creating an Employee Commission Schedule > Determine Commission Categorization and Eligibility"
parent: "section_N1123495"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1123880.html"
anchors: ["procedure_N1124080"]
sha256: "e13436eeb747be565a693440862a5a1bb0bcd1987f326cc1bca99105473fa5db"
---

You can categorize commission schedules by class, item, department, and location. When you categorize your commission schedules, NetSuite creates rows in your schedule matrix. For example, if you categorize your commission by class, NetSuite creates a row in your matrix for each class you track.

Eligible commission is defined as commission that is ready to be paid to a rep. You can choose to make commission eligible when orders are billed or paid. You can choose to have a percentage of the commission become eligible on billing, and the remainder eligible upon collection.

You can choose to have categorization apply to either payment, or both attainment and payout. For more information about how the Categorization applies to a particular field, see [Commission Attainment and Payout Categorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1129540.html). You cannot categorize commission that is calculated on transaction total.

Additionally, if you base commission on alternate sales amount (ASA) or ASA quotas, you can have commission become eligible when orders are entered (bookings).

#### To set up schedule categorization and eligibility: {#procedure_N1124080}

1.  In the **Categorized by** field, select Classes, Items, Departments, or Locations.
    
    When you select a category, NetSuite creates additional categories in the schedule matrix.
    
2.  If you base this schedule on profitability or profit, you can categorize by class, location, department, or inventory item.
    
    To track departments, locations, or classes, an administrator can go to Setup > Company > Setup Tasks > Enable Features > Company.
    
3.  In the **Categorization applies to** field, select how NetSuite applies categorization:
    
    -   **Payout Only** - NetSuite applies the percentage rate to the sales in each category to calculate commission. The commission bracket used to calculate this commission is determined by the extent to which reps attain their overall, uncategorized quota.
        
    -   **Both Attainment AND Payout** - (You must have established class, location, department, or item to select this option.) The percentage of each category's quota met by the sales rep determines the amount of commission earned.
        
    
    Note:
    
    This field is available only on schedules based on quota, ASA quota, sales, and Alt. sales and categorized by class, location, department, or item. Sales- or ASA-based schedules must use a marginal scale for this field to appear. For more information, see [Commission Attainment and Payout Categorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1129540.html).
    
4.  The **Eligible Amount** field determines when commission becomes eligible for authorization and payment:
    
    -   **Billings** - Commission is eligible when orders are billed
        
    -   **Collections** - Commission is eligible when orders are paid
        
        For more information, see [Collections-Eligible Commission and Credit Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1129338.html#bridgehead_N1129406).
        
    -   **Billings, Collections** - Commission is eligible based partially on billings and partially on collections
        
    -   **Bookings, Collections** - Commission is eligible based partially on bookings and partially on collections. This option is available on commission schedules based on ASA or ASA quotas
        
    -   **Bookings** - Commission is earned when orders are entered. This option is available on commission schedules based on ASA or ASA quotas
        
        For more information, see [Alternate Sales Amounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1049780.html).
        
5.  If commission is on ASA and the eligible amount is based on Bookings, Collections, choose how commission becomes eligible in the **Collections Eligibility** field.
    
    This field also appears for commissions based on a custom field when the **Eligible Amount** includes collections.
    
    -   **First In** - Select this option to consider the amount paid on an order to first satisfy the ASA of a transaction to satisfy commission eligibility.
        
    -   **Percent of Order** - Select this option if alternate sales amount, collections-based commission schedules determine eligibility of calculated commissions. This option bases calculated commission on the proportion of cash collected against the sales order amount, rather than the ASA total.
        
    -   **Whichever Is Greater** - Select this option to use the greater of the **First In** or **Percent of Order** amounts to determine commission eligibility.
        
    -   **Whichever Is Less** - Select this option to use the lesser of the **First In** or **Percent of Order** amounts to determine commission eligibility.
        
    
    For example, a sales order is entered for $1,000. The alternate sales amount for the order is $500.
    
    -   **First In** - The $400 payment counts toward the ASA, which makes 80% ($400/$500), or $40, eligible for commission payment.
        
    -   **Percent of Order** - The $400 payment is 40% of the order total, so 40%, or $20 of the calculated commission is eligible.
        
    -   **Whichever Is Greater** - Forty dollars is eligible because counting the payment toward the ASA gives a greater eligible amount.
        
    -   **Whichever Is Less** - Twenty dollars is eligible because counting the payment as a percentage of the order total gives a smaller eligible amount.
        
    
    The Default ASA Collections Eligibility Type preference at _Setup > Sales > Sales Management > Commissions (Administrator)_ determines the field default.
    

### Related Topics

-   [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html)
-   [Employee Commission Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1123341.html)
-   [Creating an Employee Commission Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1123495.html)
-   [Choose the Basis of the Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1123608.html)
-   [Set Commission Calculation Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1124420.html)
-   [Set Commission Schedule Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1124587.html)
-   [Create a Commission Matrix](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1124704.html)
-   [Save the Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/procedure_N1124778.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
