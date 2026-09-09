---
id: "section_N1039075"
type: "section"
title: "Updating Individual Sales Teams"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Setting Up SFA > Team Selling > Updating Individual Sales Teams"
parent: "section_N1037318"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1039075.html"
anchors: ["procedure_N1039094"]
sha256: "c1dc1fcc7197883f4cffc5a742e6535b313a4c9751473ed55306780ad63756fd"
---

You can apply changes made to sales teams to associated transactions or customer records. These changes can include removing or adding members, or changing roles and contribution percentages.

If you update the sales team on a transaction, check the Update Customer box to apply those changes to the sales team on the customer record.

If you update the sales team on a customer record, check the Update Transactions box to apply those changes to transactions for that customer.

## The following rules apply to these updates: {#procedure_N1039094}

-   NetSuite adds employees with sales rep roles with 0% contribution percentages.
    
-   NetSuite adds employees with non-sales rep roles using the contribution percentage you enter.
    
-   Employees you add to a sales team keep the sales role they already have.
    
-   Sales reps are always added as non-primary reps.
    
-   NetSuite only removes the sales team members you specifically delete from the updated record or transaction.
    
-   You can delete non-sales rep employees only if their contribution percentage is 0%.
    
-   NetSuite doesn't apply these updates to parent or child records of the updated record.
    

### Related Topics

-   [Team Selling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1037318.html)
-   [Mass Updating Sales Teams](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038939.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
