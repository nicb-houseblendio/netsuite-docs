---
id: "section_N2362161"
type: "section"
title: "Creating a Vendor Record"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Records > Vendor Record Management > Creating a Vendor Record"
parent: "article_161951406143"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html"
anchors: ["procedure_N2362198", "procedure_N2362249", "procedure_N2362395", "bridgehead_4180540809", "bridgehead_160681552484", "bridgehead_N2362466", "bridgehead_N2362537", "bridgehead_N2362621", "bridgehead_N2362678", "procedure_N2362687", "procedure_N2362784", "procedure_N2362835", "procedure_N2362870", "procedure_N2362904", "procedure_N2362970", "procedure_N2363011", "bridgehead_N2363041", "bridgehead_N2363113", "procedure_N2363139", "bridgehead_N2363155"]
sha256: "d461bb534a15cbd8d41cb4670c7ff8823a2cd355d12a624dd755684d8de8a4ec"
---

A vendor is a company or person from whom you purchase goods and services. Vendor records track information about your vendors and enable you to view past transactions and communications with them.

If you use NetSuite OneWorld, you can share a vendor record across multiple subsidiaries or assign one vendor to a single subsidiary. For more information about globally shared vendor records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).

Important:

The fields that appear in your account depend on which features you have enabled in your account. Some fields described below may not appear in your account.

#### To create a vendor record: {#procedure_N2362198}

1.  Go to _Lists > Relationships > Vendors > New_.
    
2.  Enter information as indicated below.
    
3.  Click **Save**.
    

#### Primary Information {#procedure_N2362249}

1.  In the **Custom Form** field, accept the default form or select the form you prefer to use to create this record.
    
    To customize this form, select **New** or click **Customize Form**.
    
2.  In the **Vendor ID** field, enter your vendor's name the way it should appear in all lists.
    
    -   If you leave this field blank, this field fills with the name you enter in the **Company Name** field.
        
    -   If you use Auto-Generated Numbering, this field fills with the vendor number or code.
        
3.  Next to **Vendor ID**, clear the **Auto** box to manually enter a name for this record. When this box is checked, a name or number is assigned for this record, based on your settings at Setup > Set Up Auto-Generated Numbers.
    
4.  Next to **Type**, choose whether this vendor is a company or an individual.
    
5.  In the **Company Name** field, enter the legal name of this vendor.
    
    If you use Auto-Generated Numbering, you should enter the vendor name to ensure that it appears along with the code in lists.
    
6.  In the **Web Address** field, enter a URL for this vendor's web address. When you return to this record for viewing, this address is a link.
    
7.  Select the category for this vendor.
    
    To create new categories, go to _Setup > Accounting > Accounting Lists_ . Click **Vendor Category**.
    
8.  In the **Image** field, select an image from the file cabinet to attach to this record.
    
    Click or select **New** to upload a new image.
    
9.  In the **Comments** field, enter any additional notes.
    

#### Email | Phone | Address {#procedure_N2362395}

1.  Enter the email address of your vendor. If you permit your vendors online access, this becomes part of their access code.
    
    Important:
    
    Do not give access to unknown email addresses, or unknown vendors. It is also unsafe to use generic email addresses like test@test.com.
    
2.  Enter a phone number for your vendor. It will appear on the Vendor List report.
    
3.  Enter the vendor's alternate phone number.
    
4.  Enter the vendor's fax number.
    
    You should enter the fax number exactly as it must be dialed. If a '1' is required to fax to this number, include it at the beginning of the number.
    
    The number you enter here automatically appears in the **To Be Faxed** field of transactions when you select this customer.
    
    To fax NetSuite forms, an administrator must first set up the fax service at _Setup > Company > Preferences > Printing & Fax_.
    
5.  The **Address** field automatically shows the default billing address that you enter and add using the **Address** subtab.
    

Click a subtab to schedule activities, send email, attach files, add notes and more for this vendor. For more information about choosing which fields appear on these subtabs, see [Configuring Fields or Screens](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856992.html).

## Classification {#bridgehead_4180540809}

If you use NetSuite OneWorld, in the **Primary Subsidiary** field, select the primary subsidiary to assign to this vendor.

You can"t enter transactions for this vendor unless a primary subsidiary is assigned.

The default primary currency for the vendor is the base currency of the primary subsidiary.

Note:

After you save the vendor record, you can"t change the primary subsidiary.

## Subsidiaries {#bridgehead_160681552484}

If you use NetSuite OneWorld, the **Subsidiaries** subtab enables you to assign the secondary subsidiaries that can share this vendor. After you save the vendor record, you can see vendor open balances at subsidiary level.

Note:

If the Subsidiaries subtab is not visible, your organization uses a custom vendor entry form that prevents users from associating vendors with multiple subsidiaries.

For more information, see [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html).

If this vendor record is not shared with multiple subsidiaries and for existing vendors, note the following about the **Subsidiaries** subtab. This subtab provides the primary subsidiary's outstanding balance and unbilled orders balance in the subsidiary's currency, and the vendor's credit limit.

If you have access to a vendor record and at least one assigned subsidiary, note the following. You can view and edit the vendor record, according to your permission level.

Users with access to a vendor record but not to all of the subsidiaries assigned to the vendor note the following. You can view, edit, or both only those subsidiaries to which you have access, according to your permission level.

Users with **Allow Cross-Subsidiary Record Viewing** enabled can view vendor records and all subsidiaries.

The primary subsidiary automatically displays first on this subtab.

At any time you can add a subsidiary to the shared vendor. You can delete a subsidiary if there are no associated transactions. However, if an entity shares a customer and a vendor and both are associated with a subsidiary, note the following. Any customer transaction prevents you from deleting the subsidiary assignment.

Important:

You can"t share a tax agency vendor or a vendor defined as a project resource. Further, you can"t share a vendor whose purpose is Intercompany Management.

You can deactivate an assigned subsidiary when the assignment is no longer useful to you.

When you select this vendor on a transaction, you can associate the transaction with the primary subsidiary and any or all assigned secondary subsidiaries. Note that the vendor has access to the primary subsidiary's transactions in the Vendor Center. If the Vendor Center role is customized by setting **Allow Cross-Subsidiary Record Viewing**, the vendor can see all of the transactions in the Vendor Center.

#### To configure the subsidiaries subtab:

1.  In the **Subsidiary** field, select the subsidiary that can share this vendor.
    
2.  In the **Credit Limit** field, enter the credit limit for this subsidiary.
    
    The default is no value, or no credit limit.
    
    Note:
    
    The primary subsidiary's credit limit displays in the matrix on the **Subsidiaries** subtab, rather than on the **Financials** subtab.
    
3.  In the **Tax Code** field, select the tax code to apply by default to purchase orders and bills entered for this subsidiary vendor relationship. You can change the tax code on individual transactions.
    
    If you use NetSuite OneWorld and this vendor is shared with multiple subsidiaries, note the following. You can select a tax code that is associated with any of the secondary subsidiaries assigned to this vendor.
    
    The default tax code you assign to a subsidiary vendor combination must be available on purchase transactions. Otherwise, you can"t select this tax code on purchase orders or bills for that vendor. Ensure that the **Available On** field of the tax code record (Setup > Accounting > Tax Codes) is set to **Purchase Transactions** or **Both**.
    
4.  Click **Add**.
    
    Add each subsidiary that is to share this vendor. Subsidiaries within a subsidiary do not automatically share this vendor.
    
    You can"t add multiple subsidiaries to a tax agency vendor.
    
    After you save the vendor record, the **Subsidiaries** subtab provides the primary subsidiary and any active and inactive subsidiaries. The subtab provides the outstanding balance for each subsidiary In both the currency of vendor's primary currency and the subsidiary's base currency. It also provides the unbilled orders balance in both currencies.
    
    If you use the Vendor Prepayments feature, note the following about the **Subsidiaries** subtab. This subtab provides the total balance of prepayments associated with the vendor record in the vendor's primary currency and the subsidiary's base currency.
    
    -   The **Prepayment Balance** column provides the prepayment balance in the vendor's primary currency.
        
    -   The **Prepayment Balance (Base)** column provides the prepayment balance in the subsidiary's base currency.
        

#### Relationships

1.  On the **Contacts** subtab, enter information about your contacts with this vendor.
    

#### Communication {#bridgehead_N2362466}

1.  On the **Phone Calls** subtab, view or enter new phone calls for this vendor.
    
2.  On the **Tasks** subtab, view or enter CRM tasks records relating to this vendor.
    
    For more information about tasks, see [Working with CRM Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N506499.html).
    
3.  On the **Events** subtab, enter events for this vendor.
    
4.  On the **Files** subtab, you can select and add files from the File Cabinet that are associated with this vendor. For example, you can attach a contract as a file associated with this vendor.
    
    Select **New** to upload a new file to the File Cabinet.
    
5.  On the **User Notes** subtab, add and track notations about this vendor.
    

#### Address {#bridgehead_N2362537}

1.  Check the **Default Shipping** address box if this is the main address to send returned products to the vendor.
    
2.  Check the **Default Billing** address box if this is the remittance address where payments should be sent for this vendor.
    
3.  Enter the **Label** for this address.
    
    You choose this name on transactions to select the address for this vendor.
    
4.  To add or edit values for other address fields, click the pencil icon in the **Edit** column.
    
    An address popup window displays address fields.
    
    Note:
    
    The address form shown for each employee may vary according to the country where the employee is located. It also depends on the custom address forms defined in your account.
    
    For more information, see [Customizing Address Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2874310.html).
    
    1.  Ensure the value for **Country** is correct. If it not, select a different country.
        
    2.  In the **Attention** field, enter the person at this address who should be notified of receipt of documents or goods.
        
        The value you enter automatically appears on forms if this address is marked as default for **Shipping** or **Billing**.
        
    3.  In the **Addressee** field, enter the company name that should show on the shipping label here.
        
        This name appears under the name entered in the **Attention** field.
        
    4.  Enter a phone number where the person receiving the package or mail can be reached.
        
    5.  Enter the vendor's street address.
        
        If you enter the zip code first, city and state populate automatically.
        
    6.  By default, the information entered for the address fields displays in read-only format in the **Address** free-form text box. The address fields are in the **Attention**, **Addressee**, **Address 1**, **Address 2**, **City**, **State**, **Zip**, and **Country**.
        
        To edit the read-only text, check the **Override** box.
        
    7.  Click **OK**.
        
5.  To enter additional addresses, click **Add**.
    
6.  Repeat these steps for each address for this vendor.
    

#### Marketing {#bridgehead_N2362621}

1.  The **Campaigns** subtab shows recent campaigns for this vendor.
    
2.  The **Subscriptions** subtab shows subscriptions for this vendor.
    
    -   Check the box in the **Subscribed** column next to a subscription to have this vendor be subscribed.
        
    -   Clear the box in the **Subscribed** column next to a subscription to have this vendor be unsubscribed.
        
3.  In the **Global Subscription Status** field, select the status you want to assign this vendor.
    
    If this vendor has not subscribed or unsubscribed to campaigns, you can set this status to **Soft Opt-In** or **Soft Opt-Out**. If this status is set to **Confirmed Opt-Out**, you can"t change the status.
    
    Note:
    
    Certain jurisdictions, such as the European Union (EU), have regulations about contacting entities if you do not have their explicit permission to do so. You should check that your global subscription status adheres to the regulations in the recipient's jurisdiction.
    

## Financial {#bridgehead_N2362678}

#### Account Information {#procedure_N2362687}

1.  In the **Legal Name** field, enter the legal name for this vendor for financial purposes. If you entered a name in the Company Name field, that name appears here.
    
2.  In the **Business Number** field, enter the 15-digit registration number that identifies this vendor as a client of the Canada Customs and Revenue Agency (CCRA).
    
3.  In the **Account** field, enter the account name or number for this vendor.
    
4.  Enter this vendor's legal name.
    
5.  Select a **Default Expense Account** for purchases from this vendor.
    
6.  In the **Default Payables Account** field, choose the default payable account for this vendor record.
    
7.  Select the terms you have with this vendor.
    
8.  If you have the **Multiple Currencies** feature enabled, select the currency this vendor uses.
    
    If you do business with vendors who use multiple currencies in their business dealings with you, select the vendor's primary currency. You can add additional transaction currencies on the **Currencies** subtab. For more information, see [Vendors and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1400742.html).
    
9.  In the **Terms** field, select the standard discount terms for this vendor's invoices. You can always change terms for an individual order or bill, however.
    
    To add choices to this list, go to _Setup > Accounting > Accounting Lists > New_ and click Term.
    

The primary subsidiary's credit limit displays in the matrix on the **Subsidiaries** subtab.

#### Tax Information {#procedure_N2362784}

1.  In the **Tax Reg. Number** field, enter the vendor's VAT registration number.
    
    Note:
    
    For OneWorld accounts, prior to Version 2015.1, the **Tax Code** field appeared on the **Financial** subtab. As of Version 2015.1, you specify the tax code at the line-level on the **Subsidiaries** subtab.
    
    The **Tax Code** field is not available in US edition accounts that are not OneWorld.
    
2.  Enter this vendor's **Tax ID**. This is necessary if you are required to issue a 1099 form. This number is a Social Security Number (SSN) for an individual.
    
3.  If you have paid this vendor over $600 for services this year, check the **1099 Eligible** box.
    

#### Balance Information {#procedure_N2362835}

1.  Enter the **Opening Balance** of this vendor's account.
    
2.  Enter or pick the **Date** of the balance in the **Opening Balance** field.
    
    Note:
    
    If you use NetSuite OneWorld and you have shared this vendor record with multiple subsidiaries, note the following. This section provides the vendor's open and unbilled orders balances in the both the vendor's primary currency and in the subsidiary base currency.
    

#### Project Information {#procedure_N2362870}

1.  Check the **Project Resource** box to enable this vendor to be chosen as a resource on tasks and jobs. As a job resource, a vendor can be assigned to complete a task or manage a project.
    
    Clear this box if you do not want this vendor to be chosen as a resource on tasks and jobs.
    
    Important:
    
    If you have NetSuite OneWorld, you can"t share a vendor with multiple subsidiaries and also define the vendor as a project resource.
    
2.  Select a **Work Calendar** for this vendor.
    
3.  In the **Labor Cost** field, enter the cost of labor for this vendor to be able to calculate profitability on jobs.
    

#### Schedules {#procedure_N2362904}

1.  If you use the Quantity Pricing feature, the **Schedules** subtab shows pricing schedules for this vendor.
    
    Quantity pricing schedules can be used to apply prices you have negotiated with vendors. On the **Pricing Schedules** subtab, click **New Pricing Schedule**.
    
    Only one vendor can be associated with each quantity pricing schedule. You can, however, apply a schedule to any number of items.
    
    For more information, see [Using Quantity Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2183333.html).
    

#### Transactions {#procedure_N2362970}

1.  Click **New Purchase Order** or **New Bill** to enter new transactions for this vendor.
    
2.  Existing transactions for this vendor show in the list.
    
    -   Filter the list by selecting a billing status of **Open** or **Closed**.
        
    -   Filter the list by selecting a transaction type.
        

#### Items {#procedure_N2363011}

1.  Click **Import Price List** to import a price list for this vendor.
    
2.  Items associated with this vendor show in the list.
    

#### Preferences {#bridgehead_N2363041}

1.  In the **Email Preference** field, select the format for email that is sent to this person or company. Select **Default** to use the preference set at Home > Set Preferences.
    
2.  In the **Print on Check As** field, enter the vendor name the way it should appear on a check.
    
3.  Next to **Send Transactions Via**, check the appropriate boxes:
    
    -   **Email** - Check this box to check the **To Be Emailed** box by default on transactions when this vendor is selected.
        
    -   **Print** - Check this box to check the **To Be Printed** box by default on transactions when this vendor is selected.
        
    -   **Fax** - Check this box to check the **To Be Faxed** box by default on transactions when this vendor is selected.
        
    
    For more information, see [Preferred Transaction Delivery on Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2368449.html).
    

#### System Information {#bridgehead_N2363113}

1.  The **Date Created** field displays the date this vendor record was entered.
    
2.  If you check the **Inactive** box, this vendor doesn't appear on a list unless you check the **Show Inactives** box.
    

#### System Notes {#procedure_N2363139}

1.  The **System Notes** subtab shows notations NetSuite tracks automatically.
    

You should use the following procedure that lets vendors set up a NetSuite password for themselves. However, if you prefer to set their passwords yourself, use the procedure in [Manually Setting a Vendor's Password](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162341016930.html).

#### Access {#bridgehead_N2363155}

1.  Check the **Give Access** box to give this vendor access to your NetSuite account.
    
2.  Check the **Send New Access Notification Email** box to notify your vendor of this new access. The notification email includes the email address (used for logging in to NetSuite) and explains login procedures. It also contains a URL so that the vendor can set up a NetSuite password.
    
    Checking **Send New Access Notification Email** doesn't require you to enter a password or check the **Require Password Change on Next Login** box.
    
    Note:
    
    You should let the vendor create a password for NetSuite from the URL in the notification email. However, if you prefer to assign a password for the vendor, see [Manually Setting a Vendor's Password](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162341016930.html).
    
3.  In the **Role** column, select a role for this vendor and click **Add**.
    
    If this vendor is not a contractor, assign the Vendor Center role to share purchase order and accounts payable information with your vendor.
    
    For more information, see [Assigning a Role to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2363606.html).
    

#### Time Tracking

1.  If you have given your vendor time tracking permissions, in the **Time Approver** field, select an employee to approve time tracked by this vendor.
    
    If this field is blank, time tracked by this vendor is automatically approved until entered against a project with project time approval preferences defined. For more information, see [Giving Vendors Access to Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2364581.html).
    

### Related Topics

-   [Vendor Record Configuration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161952107343.html)
-   [The Vendor Center Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2369118.html)
-   [Creating a Tax Agency Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2365187.html)
-   [Editing a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4443197067.html)
-   [Inactivating Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4443201053.html)
-   [Deleting a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4443213535.html)
-   [Merging Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4443233738.html)
-   [Vendor Dashboards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4849482517.html)
-   [Printing Mailing Labels for Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2368875.html)
-   [Vendor Record Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161951406143.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
