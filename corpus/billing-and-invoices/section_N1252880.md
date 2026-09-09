---
id: "section_N1252880"
type: "section"
title: "Creating Billing Schedules"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Advanced Billing > Creating Billing Schedules"
parent: "section_N1250607"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1252880.html"
anchors: ["procedure_N1253015"]
sha256: "32c56cb71fe94d5c801237187642baf8eeb3bd7bf5d33a8b20491aa1916e732a"
---

With Advanced Billing, you can create billing schedules for items and sales. Billing schedules define how sales are billed over time or a contract term. Billing schedules track when to invoice customers and how much to bill, managing the billing process. For example, you might bill monthly for a one-year membership or quarterly for a three-year service contract.

To create a billing schedule, define the following characteristics:

-   **Initial Amount** - the amount of the first billing instance. You can use a currency amount or a percentage of the sale total for line-level billing schedules. But percentage initial amounts are only permitted at the transaction level.
    
-   **Type** - the billing schedule type. Selecting Time and Materials or Charged-Based billing schedule types hides the Initial Amount field. When creating a billing schedule for a transaction subtotal, set this field to Standard.
    
-   **Initial Payment Terms** - payment requirements applied to the first billing instance.
    
-   **Recurrence Frequency** - how often billings repeat (for example, daily, weekly, quarterly, every four months, or monthly). When creating a billing schedule for a transaction subtotal, set this field to Custom.
    
-   **Repeat Every** - the frequency of recurring invoices. The Repeat Every field relates to the Recurrence Frequency field. Selecting Monthly for Recurrence Frequency changes the Repeat Every field to Monthly.
    
-   **Recurrence Count** - the number of bills after the first one.
    
-   **In Arrears** - bill at the end of each period, not the start.
    
-   **Recurrence Payment Terms** - payment terms for subsequent billings.
    

You can set up a billing schedule for each type of sale that incorporates the appropriate billing procedures. For example, you might create a billing schedule with an initial 50% billing amount, monthly recurrence, and two recurrences. If you apply this billing schedule to a $1,000.00 service contract sales order, it'll be billed as follows:

-   Initial invoice for 50% of the sale = $500.00
    
-   Second invoice one month later for 25% of the sale = $250.00
    
-   Third invoice one month after the second invoice for 25% of the sale = $250.00
    

Note:

The final installment is calculated differently than the others. The final installment in a billing schedule is calculated as:

Final installment = Total amount - (sum of all other installments and initial amount)

To apply a billing schedule to a subtotal, set the **Type** field to **Standard**, set the **Recurrence Frequency** field to **Custom**, and check the **Apply to Subtotal** box.

#### To create a billing schedule: {#procedure_N1253015}

1.  Go to _Lists > Accounting > Billing Schedules > New_.
    
2.  In the **Name** field, enter a name for this schedule.
    
    For example, you might name the schedule **50% down, 2 monthly**.
    
3.  In the **Initial Amount** field, enter the initial billing amount. You can enter this amount as a currency amount or as a percentage. This can be a currency amount or a percentage of the sale total if you use line-level billing schedules. You can only use percentage initial amounts at the transaction level.
    
4.  In the **Initial Payment Terms** field, select the terms to be used on the first invoice to be created from the sales order.
    
    To add new payment terms, go to _Setup > Accounting > Setup Tasks > Accounting Lists > New > Term > New_ > Term > New.
    
5.  In the **Recurrence Frequency** field, select the frequency for bills to recur.
    
    Select **Custom** to create a new frequency or to create a billing schedule you want to apply to the subtotal of a transaction:
    
    Define the frequency by entering information in the middle fields.
    
    1.  In the **Count** field, enter the number of units of time to calculate a billing date.
        
        For example, enter **12** to bill twelve months after the initial bill.
        
    2.  In the **Units** field, enter the units of time to calculate a billing date.
        
        For example, select **Months** to bill twelve months after the initial bill.
        
    3.  By default, billing frequency is based on the initial invoice date. You can use the Relative to Previous box to base subsequent bills on the previous bill's date instead of the initial invoice date.
        
        Check the **Relative to Previous** box if the frequency is relative to the previous billing instead of the transaction date.
        
        The Relative to Previous box doesn't affect the first bill line, which is always based on the initial bill. Checking or clearing the box affects the bill date for subsequent bill lines.
        
        For example, if a sales order's initial invoice is created on 01/01/2007:
        
        The first line in the bill schedule has a Count and Units of 1 Month. This bill will be created on 02/01/2007.
        
        The second line in the bill schedule has a Count and Units of 2 Months. If Relative to Previous is checked, this bill is scheduled for 2 months after the previous line, or 04/01/2007. If Relative to Previous is cleared, this bill is scheduled for 2 months after the initial bill, or 03/01/2007.
        
        When you check the Relative to Previous box, the date of that billing appears in the Example field.
        
    4.  In the **Amount** field, enter the amount to be billed. This can be a currency amount or a percentage of the sale total if you use line-level billing schedules, but you can only use percentage initial amounts if you apply billing schedules on the transaction level.
        
6.  If you selected a Recurrence Frequency other than custom, enter a Recurrence Count. This defines the number of invoices or cash sales generated after the initial sale. The remaining amount due for the sale (after the initial amount is deducted) is evenly divided between the recurring invoices.
    
    For example, the total to be billed for a sale is $2,400.00. The billing schedule applied to the sale has an initial amount of 50%, a recurrence frequency of monthly, and a recurrence count of 12. The initial invoice total is $1,200.00 and then a recurring invoice of $100.00 is generated one time per month for 12 months to bill the remainder of the sale.
    
7.  In Arrears will be checked by default.
    
    -   When In Arrears is checked, billing occurs at the end of the recurrence period.
        
        From the example in step 6, if the initial invoice for $1,200.00 is generated on January 1st, 2006, then the first recurring monthly invoice for $100.00 is generated on February 1st, 2006.
        
    -   When In Arrears is cleared, billing occurs at the beginning of the recurrence period.
        
        From the example in step 6, if the initial invoice for $1,200.00 is generated on January 1st, 2006, then the first recurring monthly invoice for $100.00 is also generated on January 1st, 2006. NetSuite combines these two amounts on one invoice, so the first invoice includes both the initial amount and the first recurring payment, for an invoice total of $1,300.00.
        
8.  In the **Recurrence Payment Terms** field, select the terms to be used on all invoices subsequent to the initial invoice.
    
    Note:
    
    This field is greyed out when you select Custom in the Recurrence Frequency field.
    
9.  If you do not want this schedule to be applied to items and new orders, inactivate the schedule by checking the **Schedule is Inactive** box.
    
10.  Click **Save**.
     

It is possible to create a billing schedule that will bill more than 100% of the invoice amount.

For example, you could create a schedule for the initial amount of $10,000.00 and then a custom frequency of 25% billed every three months. If you apply this schedule to an order totaling $60,000.00, the invoices are created as below:

-   1st invoice = $10,000.00
    
-   2nd invoice = $12,500.00
    
-   3rd invoice = $12,500.00
    
-   4th invoice = $12,500.00
    
-   5th invoice = $12,500.00
    
-   **Total billed = $60,000.00**
    

After the initial amount, invoices are created based on 25% of the total bill, not based on the remainder due after the initial amount. If your schedule uses both dollar amounts and percentages, or uses a custom frequency, verify that the total amount billed by the schedule is the amount intended.

Note:

Billing schedules created using the above steps default to be Private and cannot be set to Public.

Private billing schedules show only in the transaction it is created from.

Public billing schedules show on any transaction.

To create a Public billing schedule, it must be created on the fly. Read [Creating Billing Schedules From an Estimate or Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253492.html).

### Related Topics

-   [Advanced Billing Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1250795.html)
-   [Enabling Advanced Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1251128.html)
-   [Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1251398.html)
-   [Applying Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253848.html)
-   [Discount and Markup Items and Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254542.html)
-   [Billing Customers Using Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254744.html)
-   [Viewing Invoice Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256403.html)
-   [Advanced Billing and Advanced Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1256787.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
