---
id: "chapter_N3265696"
type: "chapter"
title: "Button IDs"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript IDs > Button IDs"
parent: "chapter_1494647249"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3265696.html"
anchors: []
sha256: "503eb7296813317b0a8378bb7f3cca64f399c7f488c6e53319c1c7478ceae576"
---

The following table lists the internal IDs for standard NetSuite buttons that support SuiteScript.

These buttons may appear as inline buttons or as actions in the Actions menu for some records. The following properties of the [serverWidget.Button](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4325806317.html) object can be used to customize buttons and actions:

-   [Button.label](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4325807686.html) - Use this property to change the label of the button or action.
    
-   [Button.isHidden](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4325806318.html) - Use this property to hide or show the button or action.
    

You cannot use SuiteScript to do the following:

-   Change the display type of a button from an inline button to an action in the Actions menu, or from an action to an inline button.
    
-   Add or remove a custom button to or from the Actions menu.
    

You can use point-and-click customization to change the display type of buttons and actions. For more information, see [Configuring Buttons and Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2857647.html).

Important:

Customizing the Save, Edit, Cancel, Back, and Reset buttons is not supported in SuiteScript or in point-and-click customization.

| Button UI Label | Button Internal ID |
| --- | --- |
| Add Items | addmatrix |
| Accept | accept |
| Accept Payment | acceptpayment |
| Apply | apply |
| Approve | approve |
| Approve Return | approvereturn |
| Authorize Return | return |
| Auto Fill | autofill |
| Bill | bill |
| Bill Remaining | billremaining |
| Cancel Order | cancelorder |
| Cancel Return | cancelreturn |
| Clear Splits | clearsplits |
| Close | closeremaining |
| Convert | convertlead |
| Convert to Inventory | convertinvt |
| Convert to Lot Numbered Inventory | convertlot |
| Convert to Serialized Inventory | convertserial |
| Create Build | createbuild |
| Create Matrix | creatematrix |
| Credit | credit |
| Decline | decline |
| Delete | delete |
| Email | email |
| Fax | fax |
| Fulfill | process |
| Generate Price List | generatepricelist |
| Generate Statement | generatestatement |
| GL Impact | glimpact |
| Go To Register | gotoregister |
| Grab | grab |
| Make Copy | makecopy |
| Make Payment | payment |
| Make Standalone Copy | makestandalonecopy |
| Memorize | memorize |
| Merge | merge |
| New | new |
| New Event Field | neweventfield |
| Next Bill | nextbill |
| Next Week | next |
| Prev Week | prev |
| Print | print |
| Print Bill of Materials | printbom |
| Print Label | printlabel |
| Print Labels | printlabels |
| Print Picking Ticket | printpicktick |
| Print Summary | depositsummary |
| Quick Accept | quickaccept |
| Recalc | recalc |
| Receive | receive |
| Refund | refund |
| Reject | reject |
| Renew | renewal |
| Reset | resetter |
| Revenue Commitment Reversal | revcomrv |
| Save As | submitas |
| Save & Bill | submitbill |
| Save & Convert | submitconvert |
| Save & Copy | submitcopy |
| Save & Edit | submitedit |
| Save & Email | saveemail |
| Save & Fulfill | submitfulfill |
| Save & New | submitnew |
| Save & Next | submitnext |
| Save & Print | saveprint |
| Save & Print BOM | saveprintbom |
| Save & Print Label | saveandprintlabel |
| Save & Refund | submitrefund |
| Save & Same | submitsame |
| Save Baseline | savebaseline |
| Search | search |
| Show Activity | showactivity |
| Submit Invoice | submitinvoice |
| Tentative | tentative |
| Unbuild | createunbuild |
| Update Matrix | updatematrix |
| Update VSOE | updatevsoe |
| View All Transactions | viewalltransactions |
| Void | void |
| W4 Worksheet | w4data |

### Related Topics

-   [SuiteScript IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1494647249.html)
-   [Permission Names and IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3236764.html)
-   [Feature Names and IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3247851.html)
-   [Preference Names and IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3251359.html)
-   [Task IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3269064.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
