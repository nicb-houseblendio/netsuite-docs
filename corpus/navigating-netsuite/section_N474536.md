---
id: "section_N474536"
type: "section"
title: "Popup and Dropdown Lists"
branch: "navigating-netsuite"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Navigating NetSuite > Popup and Dropdown Lists"
parent: "section_N474404"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N474536.html"
anchors: ["bridgehead_N474548", "bridgehead_N474560", "bridgehead_N474619", "bridgehead_N474758", "bridgehead_N474692", "bridgehead_N474723"]
sha256: "1ace5fe6b06d45e3e841c1172f33c03b7e4bf364f389a3783080658ad9cc4a88"
---

When you're selecting from a long list of records in a NetSuite field, you can use built-in features like autocompletion and popup lists to save time. These functions include autocompletion and popup lists. Many fields also include links to search, edit, and create related records.

-   [Autocompleting Dropdown Lists](#bridgehead_N474548)
    
-   [Accessing Related Records from Dropdown Lists](#bridgehead_N474560)
    
-   [Using Popup Lists](#bridgehead_N474619)
    
-   [Using Popup List Search Links](#bridgehead_N474758)
    
-   [Popup Multi-Select Lists](#bridgehead_N474692)
    
-   [Using Popup Auto Suggest](#bridgehead_N474723)
    

## Autocompleting Dropdown Lists {#bridgehead_N474548}

Instead of selecting from a dropdown list, you can type the first letters of a value and the field is completed automatically.

## Accessing Related Records from Dropdown Lists {#bridgehead_N474560}

Some dropdown lists include buttons to access related records, so you can quickly add, review, or change a record before you select it for a field. These buttons appear when you hover over the dropdown list.

-   Click the new ![Add New icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/NavigatingNetSuite_AddNewIcon.png) button to create a new record in a popup window.
    
-   Click the open button ![Open icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/WorkingWithRecords_OpenIcon.png) to view or edit an existing record. The record opens in view mode in a new tab. Click **Edit** on the record to change to edit mode.
    

## Using Popup Lists {#bridgehead_N474619}

You can use the Maximum Entries in Dropdowns preference to force popup lists instead of dropdown lists for fields with large numbers of possible values. To set this preference, go to _Home > Set Preferences_. The Maximum Entries in Dropdowns field is on the General subtab. Enter the maximum number of records you want to appear in a dropdown list. If the possible values in a list exceeds this number, the list automatically becomes a popup list. If the possible values don't exceed this number, a dropdown list appears.

Tip:

Enter **0** in the **Maximum Entries in Dropdowns** field to always use popup lists. To always use dropdown lists, enter a large number that exceeds the number of entries in any of your lists.

Each popup list includes double arrows ![Double Arrow icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/NavigatingNetSuite_DoubleDownArrows.png) in place of the single arrow for a dropdown list. Start typing and press the Tab key to open a popup window that contains only records that begin with the letters you typed. For example, in the following screenshot, a user typed 'wol' and pressed Tab to display a list of customers.

![Example of a list.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/PopupList_AutoSuggest.png)

Alternatively, you can click the double arrows to display a popup and choose to open a list or search. The new and open buttons also appear when you click the arrows as shown in the following screenshot.

![List and Search options.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/DropdownList_PopupList.png)

-   Click the new button to open a popup window and add a new record.
    
-   Click the open button to open the selected record in view mode in a new tab. Click **Edit** on the record to change to edit mode.
    

To clear a value that you've previously entered in the list, select the value and press the Delete key.

## Using Popup List Search Links {#bridgehead_N474758}

Most fields with a popup list also have a search link. Click the **Search** icon, and a search window pops up. Enter criteria for the search, click Submit, and you'll see a list of items matching your search criteria. Select the item you want, and it'll be added into the field.

For example, to create a sales order for a customer in Alaska, click **Search** next to the Customer:Project field. When the Customer Search window pops up, type AK in the state field, and click Submit. The pop up window changes to show only your customers in Alaska. Click the name of the customer you want, and NetSuite inserts it into the Customer:Project field.

On transaction forms, NetSuite searches the full name of the item or the name of the final subitem and autofills the item field with any matching names. For example, if you type **bas** you'll find Summer:Picnic:Basket and Basket:Welcome.

Note:

After you inactivate a record, it won't show on transactions for selection in popup or dropdown lists. However, if the Search option appears in the popup or dropdown for a field, the search will return inactive records if the Inactive filter is set to Either or Yes. Inactive records in these search results can be added to transactions. To filter inactive records out of search results, be sure to set the Inactive filter to No in the search criteria.

## Popup Multi-Select Lists {#bridgehead_N474692}

On fields that allow you to select multiple values, you can access popup multi-select lists. To quickly enter a single value in this type of field, type the first few letters and press Tab. To enter multiple values, click the double arrow button to display a popup with a complete list of records that you can select and search.

![Multi-select field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/NavigatingNetSuite_MultiSelect.png)

To search for records, enter the first letters of the record name and click **Search**. To add fields to your selection, click the record name in the left column. The item moves to the Current Selections column on the right.

![Multi-select popup window.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/NavigatingNetSuite_NoSelections.png)

When you've selected all required records, click **Done**.

![Multi-select popup window with the Done button highlighted in red.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/NavigatingNetSuite_MultiSelectPopup.png)

Note:

To change or remove values in a multi-select list, don't edit the list directly. Click the double arrow button to open the popup and make the required changes.

To remove a value from a multi-select list, click the double arrow button beside the field.

![Multi-select icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/NavigatingNetSuite_MultiSelectEdit.png)

Click the X button next to the selection that you want to remove, and then click **Done**.

![Multi-select popup window with items selected.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/NavigatingNetSuite_MultiSelectEditList.png)

## Using Popup Auto Suggest {#bridgehead_N474723}

NetSuite provides an auto suggest function for popup lists. As you type three letters or more, a list of suggested matching records appears. You can select from this list to quickly populate the field.

![Search field with suggestions.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/Dropdown_AutoSuggest.png)

If you don't want to see suggested matches, you can disable the auto suggest feature by clearing the Popup Auto Suggest box on the Analytics subtab of Home > Set Preferences.

### Related Topics

-   [Navigating NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N474404.html)
-   [Finding Your NetSuite Account ID](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1498754928.html)
-   [Header and Menus](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N474479.html)
-   [Centers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164208316196.html)
-   [Dashboards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4320707520.html)
-   [Global Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4307693953.html)
-   [Create New Menu](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N588325.html)
-   [QuickViews](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N474793.html)
-   [Keyboard Shortcuts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N474926.html)
-   [Buttons and Menus in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180852421.html)
-   [Text Enhance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2171112518.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
