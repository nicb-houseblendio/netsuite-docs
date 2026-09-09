---
id: "section_N2386460"
type: "section"
title: "Creating a Vendor Return Authorization"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Returns > Creating a Vendor Return Authorization"
parent: "chapter_N2386193"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2386460.html"
anchors: ["bridgehead_N2386529", "procedure_N2386676", "procedure_4364565079", "procedure_N2386762", "procedure_N2386786"]
sha256: "45f6a4f410090e1b7ee3706fc7da11ae588eaa6729dfe26bf798870cdaf2f31e"
---

NetSuite offers two ways to create a vendor return authorization:

-   Create an individual vendor return authorization.
    
-   Create a vendor return authorization from an existing purchase order.
    
    This creates a vendor return authorization that automatically shows the items and prices from the original purchase.
    

Tip:

To print a Vendor Return Authorization form you must be in View mode.

Note:

After you enter a quantity for an item on a vendor return authorization, note the following about changing the quantity later:

-   Returning fewer items than you ordered is allowed.
    
-   Do not increase the quantity or change the rate because it will create an improper G/L impact.
    

#### To create an individual vendor return authorization: {#bridgehead_N2386529}

1.  Go to _Transactions > Purchases > Enter Vendor Return Authorizations_.
    
2.  Complete the form as described in the sections below.
    
3.  Click **Save**.
    
    After you click **Save**, the vendor return authorization is recorded in the Vendor Return Authorizations register, a non-posting account in your chart of accounts.
    

#### Primary Information

1.  The **Subsidiary** field displays the subsidiary associated with this transaction.
    
    Note:
    
    This field appears only if you use NetSuite OneWorld. If you have defined vendor records that are shared with multiple secondary subsidiaries, you can change the subsidiary where the vendor return is authorized. For more information about globally shared vendor records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).
    
2.  Optionally enter a reference number for this return transaction. Typically, this is a number provided by the vendor after they approve the return. This number may be referred to by the vendor as an RMA number or return number.
    
3.  Select a vendor.
    
    If this vendor is shared with multiple secondary subsidiaries, the **Vendor** field lists all of the vendors assigned to the selected subsidiary.
    
4.  The status of the approval can be one of the following:
    
    -   Pending Approval
        
    -   Pending Return
        
        Note:
        
        By selecting Pending Return, the authorization skips the approval process.
        
    
    If your company uses the approval process for vendor return authorizations, Pending Approval is your default status. If your company doesn't use the approval process, Pending Receipt is your default status.
    
    The default status for return authorizations is set by an administrator at Setup > Accounting > Accounting Preferences on the **Order Management** subtab. You can change the status for each vendor return authorization in this field, if needed.
    
5.  Accept or enter the date.
    
6.  The vendor's currency appears in the **Currency** field. All currency amounts on this transaction are shown in this currency.
    
7.  The currency's exchange rate is shown in the **Exchange Rate** field. You can edit the exchange rate for this transaction only, or you can update the currency record with the exchange rate you enter here.
    
8.  In the **Memo** field, you can enter information about this return, such as the reason for the return. What you enter in this field appears on reports.
    

#### Classification

1.  Select a department, class or location if you track them.
    

#### Expenses and Items {#procedure_N2386676}

1.  On the **Expenses** subtab, select an account to associate with this vendor return.
    
2.  Enter expenses associated with this return that you want to show on a vendor credit when this return is fulfilled.
    
    Both items and expenses show on a vendor credit. However, only items show on a return fulfillment. Expenses **do not show** on return fulfillments.
    
3.  If this expense is for a particular customer, select that customer in the **Customer** column.
    
    Note:
    
    If you use NetSuite OneWorld and the selected customer is shared with multiple subsidiaries, you can choose any customer associated with the selected subsidiary. For information about sharing customer records with multiple subsidiaries, see [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
    
4.  Click **Add** after each entry.
    
5.  Click the **Items** subtab and select the item you are returning.
    
6.  Enter information about items being returned:
    
    1.  Click **Add Multiple** to add several items to this transaction.
        
        The Choose Item window opens and shows a list of items you can add.
        
    2.  Filter the list by item type or name.
        
    3.  In the left pane, click an item to add it to the right pane.
        
    4.  Enter an item **Quantity**.
        
    5.  Click **Done**.
        
        Items and quantities shown in the right pane are added to the transaction.
        
    
    If the item being returned is a serialized item:
    
    1.  Enter the item number in the **Item** field.
        
    2.  Click **List**.
        
    3.  Select the serial number purchased from the vendor you chose in the **Vendor** field.
        
    4.  Enter the serial number and the item number automatically fills the **Item** field.
        
7.  If this item is for a particular customer, select that customer in the **Customer** column.
    
    If the selected customer is shared with multiple subsidiaries, you can choose any customer associated with the selected subsidiary.
    
8.  Click **Add** after each entry.
    

#### Billing {#procedure_4364565079}

1.  Click the **Billing** subtab.
    
2.  In the **Vendor Select** field, choose a vendor.
    
3.  Verify the billing address displayed in the **Vendor** field. To change the address, click the Edit button to the right of the Vendor Select field.
    

#### Relationships {#procedure_N2386762}

1.  The primary contact for the vendor is selected automatically. To edit information for this contact, click the contact's name.
    
2.  You can also add contacts to this order by entering the contact's information and clicking **Add**.
    

#### Communication {#procedure_N2386786}

1.  Use the **Events**, **Tasks**, and **Phone Calls** subtabs to attach activities to this transaction. For more information, see [Attaching Events, Tasks, and Calls to Records and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1084924.html).
    
2.  On the **Files** subtab, you can select and attach files from the File Cabinet related to this transaction. Select **New** to upload a new file to File Cabinet.
    
3.  On the **User Notes** subtab, you can enter a title and note for any comments you want to add to this transaction. Click **Add** after each note.
    

### Related Topics

-   [Vendor Return Authorization Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2386202.html)
-   [Creating a Vendor Return Authorization From an Existing Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162003965369.html)
-   [Approving a Vendor Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2387067.html)
-   [Canceling a Vendor Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162004032986.html)
-   [Shipping Authorized Vendor Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2387332.html)
-   [Viewing the Status of a Vendor Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2387708.html)
-   [Crediting an Authorized Vendor Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2388089.html)
-   [Vendor Returns for Drop-Ship Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2391620.html)
-   [Closing a Line Item on a Vendor Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2391809.html)
-   [Vendor Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2386193.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
