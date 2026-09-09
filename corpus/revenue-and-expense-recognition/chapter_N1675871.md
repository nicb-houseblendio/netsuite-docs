---
id: "chapter_N1675871"
type: "chapter"
title: "Revenue and Expense Recognition Overview"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Revenue and Expense Recognition Overview"
parent: "book_N1675734"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1675871.html"
anchors: []
sha256: "e57d451f8bc3a9937166d47eee2b00a8a8611408df62ce58a3460c69f18b0001"
---

Revenue recognition features let you recognize revenue independently from billing customers and receiving payments to defer revenue for recognition in multiple future time periods. The amortization feature lets you record expenses independently from receiving bills and making payments, so you can defer expenses and spread their impact across multiple future time periods.

NetSuite currently offers the following revenue and expense recognition features:

-   **Advanced Revenue Management in Configuration Mode**
    
    This feature lets you configure ARM (Essentials) and ARM (Revenue Allocation) without affecting your current revenue recognition process. Transactions **aren't** processed using ARM while this feature is enabled.
    
    ARM in Configuration Mode is automatically enabled when you enable the ARM (Essentials) feature. Enabling this feature doesn't change your revenue recognition workflow. If you're using the classic Revenue Recognition feature, then your transactions continue to be processed through that feature and all revenue recognition reports remain available.
    
    See [Advanced Revenue Management in Configuration Mode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0726035100.html).
    
-   **Advanced Revenue Management (Essentials)**
    
    This feature automates revenue forecasting, recognition, reclassification, and auditing through a rule-based event handling framework. With Advanced Revenue management (Essentials) you can defer revenue for recognition across future periods according to the rules you configure.
    
    The Accounting Periods feature must be enabled as a prerequisite for Advanced Revenue Management (Essentials).
    
    See [Advanced Revenue Management (Essentials) and (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4328435538.html).
    
-   **Advanced Revenue Management (Revenue Allocation)**
    
    The Advanced Revenue Management (Revenue Allocation) is an add-on feature to Advanced Revenue Management (Essentials). This feature supports the use of fair value pricing, range checking, and fair value formulas to allocate revenue across several performance obligations.
    
    The Advanced Revenue Management (Revenue Allocation) feature supports fair values based on vendor-specific objective evidence (VSOE), best estimate of selling price (ESP), third party evidence (TPE), and other fair value methods your company uses. These fair values are used to determine the revenue allocation ratios for multi-element transactions.
    
    The Advanced Revenue Management (Essentials) feature must be enabled as a prerequisite for Advanced Revenue Management (Revenue Allocation).
    
    See [Advanced Revenue Management (Essentials) and (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4328435538.html).
    
-   **Revenue Recognition Approval Workflow**
    
    This SuiteApp adds approval workflow to advanced revenue management. It manages the validation and approval routing of revenue arrangements before they are further processed. You can customize the workflow to add and remove features based on your business requirements.
    
    See [Revenue Recognition Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4436595812.html).
    
-   **Rule-Based Recognition Treatment**
    
    When Advanced Revenue Management (Essentials) is enabled, you can also enable the Rule-Based Recognition Treatment feature. This feature enables you to define recognition treatments and recognition treatment rules that determine revenue recognition attributes for revenue elements based on specified criteria.
    
    See [Rule-Based Recognition Treatment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1552502028.html).
    
-   **Amortization**
    
    When this feature is enabled, you can create amortization templates that use standard or custom amortization methods, and you can associate these templates with items or transactions.
    
    When a NetSuite user enters a purchase transaction, a schedule is generated to recognize expenses based on the template associated with the item or transaction. The schedule enables you to post the appropriate journal entries to the general ledger to record expenses in future periods. For example, if your company must pay for an annual software license before the license period begins, you most likely will want to spread recognition of the license expenses throughout the following year.
    
    See [Expense Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1765678.html).
    

The following NetSuite revenue recognition features were available in the past and are still supported for customers who have previously enabled them:

-   **Revenue Recognition**
    
    When this feature is enabled, you can create revenue recognition templates that use standard or custom recognition methods, and you can associate these templates with items.
    
    For each sales transaction that includes items with associated revenue recognition templates, one or more revenue recognition schedules are generated. These schedules are based on the templates associated with the items sold. You use these revenue recognition schedules to post the appropriate journal entries to the general ledger to recognize revenue in future periods. For example, if customers have to pay in advance for a service, such as an annual maintenance contract, then you'd periodically recognize revenue after billing the customer and receiving payment, according to the associated template and schedule.
    
    See [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html).
    
    The Revenue Recognition feature must be enabled to enable and use other revenue features.
    
-   **Revenue Commitments**
    
    This feature lets you recognize revenue **before** issuing an invoice to a customer. For example, if customers don't have to pay for services until your company fulfills certain milestones, such as phases of a construction project, then you may have to recognize revenue after incurring significant costs, but before you can bill the customer. Also, due to timing differences, the amount recognized may not equal the amount billed for a specific period.
    
    See [Using Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1701780.html).
    
-   **VSOE**
    
    This feature lets you accurately recognize revenue to meet the requirements of vendor-specific objective evidence (VSOE) accounting standards. VSOE standards provide guidelines for recognizing revenue from a bundle of products and services. Each of the items in the bundle may be invoiced as part of the bundle, but may also have independent market prices. For revenue recognition purposes, VSOE resolves the discrepancy between an item's bundle price and its fair market value.
    
    VSOE is often used to recognize revenue for computer system projects that include hardware purchases, software licenses, implementation services, and maintenance contracts.
    
    See [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html).
    
-   **EITF 08-01 Revenue Recognition**
    
    EITF 08-01 Revenue Recognition automates the complex pricing calculation and revenue allocation processes required to comply with the Financial Accounting Standards Board (FASB) rules for Emerging Issues Task Force (EITF) Rule 08-01. This rule requires companies that sell products and services with multiple elements to report both recurring and non-recurring revenue items based on estimated selling prices.
    
    This feature is available with the NetSuite SuiteApp 29321.
    
    See [EITF 08-01 Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1742394.html)
    
-   **Sales Order Revenue Forecasting**
    
    This feature lets you forecast revenue using sales orders and return authorizations, so that forecast amounts include billed, unbilled, and deferred revenues. This method can provide a more complete forecast.
    
    See [Using Sales Order Revenue Forecasting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1750747.html).
    

### Related Topics

-   [Accounting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/set_N1379402.html)
-   [General Accounting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710627041.html)
-   [Banking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_4289362044.html)
-   [Taxation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4316106593.html)
-   [Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N2092473.html)
-   [Fixed Assets Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710626334.html)
-   [Statistical Accounting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3842166657.html)
-   [Multi-Book Accounting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_3831565332.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
