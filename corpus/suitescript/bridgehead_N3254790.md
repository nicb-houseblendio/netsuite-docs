---
id: "bridgehead_N3254790"
type: "bridgehead"
title: "User Preferences"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript IDs > Preference Names and IDs > User Preferences"
parent: "chapter_N3251359"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3254790.html"
anchors: []
sha256: "421fb8ca62189003b138fc24a631ee29c897dd233cfa95cd6d11d01808523c58"
---

These are the user preferences that can be found by going to _Home > Set Preferences_.

The internal ID for the user preferences page (which appears as the Set Preferences page in the UI) is **userpreferences**. All preference internal IDs are case-sensitive.

Be aware that the API for setting user preferences works the same as the UI in terms of setting a preference for a user's session or setting it permanently. In the UI if a user sets a preference, and the preference reverts back to a default setting on the user's next login, the same behavior is supported in SuiteScript.

| Preference UI Label | Preference Internal ID |
| --- | --- |
| **On the General tab** |
| Nickname | MESSAGE\_NICKNAME |
| Signature | MESSAGE\_SIGNATURE |
| Add Signature to Messages | MESSAGE\_AUTOSIGNATURE |
| From Email Address | MESSAGE\_EMAIL |
| Language | LANGUAGE |
| Search Sorting | SEARCHSORTING |
| Language of the Help Center | HELP\_LANGUAGE |
| PDF Language | PDFLANGUAGE |
| Time Zone | TIMEZONE |
| First Day of the Week | FIRSTDAYOFWEEK |
| Date Format | DATEFORMAT |
| Long Date Format | LONGDATEFORMAT |
| Time Format | TIMEFORMAT |
| Number Format | NUMBERFORMAT |
| Negative Number Format | NEGATIVE\_NUMBER\_FORMAT |
| Phone Number Format | PHONEFORMAT |
| Auto Place Decimal | AUTOPLACE |
| CSV Column Delimiter | CSV\_COLUMN\_DELIMITER |
| CSV Decimal Delimiter | CSV\_DECIMAL\_DELIMITER |
| Use Multicurrency Expense Reports | USE\_MC\_ON\_EXPREPT |
| Download PDF Files | DOWNLOADPDFS |
| Address Mapping Type | MAPTYPE |
| Show Internal IDs | EXPOSEIDS |
| Only Show Last Subaccount | ONLYSHOWLASTSUBACCT |
| Only Show Last Subentity | ONLYSHOWLASTSUBENT |
| Only Show Last Subitem | ONLYSHOWLASTSUBITEM |
| Submit Warnings | SUBMITWARNINGS |
| Limit CC Field to Contacts & Employees | EMAILLIMITCC |
| Default Issue Email Notification | ISSUE\_EMAIL\_ME\_WHEN |
| Notify Me Upon Issue Assignment | ISSUE\_NOTIFY\_UPON\_ASSIGNMENT |
| Delay Loading of Sublists | DELAYLOADINGSUBLISTS |
| Number of Rows in List Segments | LISTSEGMENTSIZE |
| Maximum Entries in Dropdowns | MAXDROPDOWNSIZE |
| Type-Ahead on List Fields | TYPEAHEADSELECTS |
| Require Exact Match on Item Type-Ahead | ITEMEXACTMATCH |
| Show Quick Add Row on Lists | SHOWQUICKADD |
| Display Bounce Warning on Campaigns | CAMPAIGN\_BOUNCE\_WARNING |
| Prefer Native Select Fields Over NS Dropdowns in Internet Explorer | NATIVE\_DROPDOWNS |
| Show App ID Field | SHOW\_APPID\_FIELD |
| Show ID Field on Sublists | SHOW\_ID\_FIELD |
| **On the Appearance tab** |
| Color Theme | COLORTHEME |
| Screen Font | FONT |
| Compensate for Large Fonts | SYSTEMLARGEFONTS |
| Density Setting for Internet Explorer | MSIE\_ZOOM\_FACTOR |
| Register Look on Lists | REGISTERSTYLE |
| Only Show Field Boarders on Hover | SHOWFIELDBORDERONHOVER |
| Chart Theme | CHART\_THEME |
| Chart Background | CHART\_BACKGROUND |
| Landing Page | LANDINGPAGE |
| Show Portlet Hint | SHOWPORTLETHINT |
| Set Customer Dashboard As Default View On Customer Record | DASHBOARD\_DEFAULT\_VIEW\_FOR\_CUSTOMER |
| Limit Entry Forms to Two Columns | LIMITTOTWOCOLUMNS |
| Expand Tabs on Entry Forms | UNLAYEREDTABS |
| Enable Rich Text Editing | RICHTEXTEDITOR |
| Default Rich Text Editor Font | EDITORFONT |
| Default Rich Text Editor Font Size | EDITORFONTSIZE |
| Display Default Them With Optimal Color Contrast | ACCESSIBILITY\_HIGH\_CONTRAST |
| **On the Transactions tab** |
| Auto Fill Transactions | AUTOFILL |
| Alphabetize Items Regardless of Type | ALPHABETIZE\_ITEMS |
| Duplicate Number Warnings | DUPLICATEWARNINGS |
| Inventory Level Warnings | STOCKWARNINGS |
| Customer Credit Limit Handling | CUSTCREDLIMHANDLING |
| Vendor Credit Limit Warnings | VENDCREDLIMWARNINGS |
| Print Using HTML | HTMLPRINTING |
| Transaction Email Attachment Format | TRANSACTION\_ATTACHMENT\_FORMAT |
| Horizontal Print Offset | HORZPRINTOFFSET |
| Vertical Print Offset | VERTPRINTOFFSET |
| **On the Analytics tab** |
| Report by Period | REPORTBYPERIOD |
| Show Reports in Grid | REPORTGRID |
| Customize Font on Financial Reports | ENABLE\_REPORT\_FONT\_CUSTOMIZATION |
| Print Company Logo | DISPLAYLOGO |
| Display Report Title on Screen | DISPLAYRPTTITLE |
| Display Report Description | DISPLAYRPTDESC |
| Calculate Forecasts as Weighted | FORECASTWEIGHTED |
| Default Bank Account | DEFAULT\_BANKREG |
| Show Forecasts as Weighted | FORECASTWEIGHTED |
| Show List When Only One Result | SHOWLISTONERESULT |
| Quick Search Uses Keywords | KEYWORDSEARCH |
| Popup Search Uses Keywords | KEYWORDSEARCHPOPUP |
| Include Inactives in Global & Quick Search | SEARCHINACTIVES |
| Popup Auto Suggest | POPUPAUTOSUGGEST |
| Global Search Auto Suggest | SEARCHAUTOSUGGEST |
| Global Search Sort by Name/ID | GLOBALSEARCHSORTBYNAME |
| Global Search Customer Prefix Includes Leads and Prospects | GLOBALSEARCHCUPREFIX |
| PDF Page Orientation | REPORTPDFORIENTATION |
| PDF Font Size | REPORTPDFFONTSIZE |
| CSV Export Character Encoding | CSVEXPORTENCODING |
| KPI Export Character Encoding | KPI\_PERIOD\_SPECIFIC\_RATES |
| **On the Activities tab** |
| Edit Activities from Calendar | EVENT\_EDITFROMCALENDAR |
| Send Invitation Emails | EVENT\_EMAILNOTIFICATION |
| Restrict Invitees to Employees | EVENT\_INTERNALINVITEESONLY |
| Default Event Access Setting for New Events | EVENT\_DEFAULTPUBLIC |
| Default Reminder Type | REMINDERTYPE |
| Default Reminder Time | REMINDERPERIOD |
| Play Audio with Popup Event Reminders | REMINDERPLAYWAVE |
| Default Priority for Tasks | DEFAULTTASKPRIORITY |
| Default New Tasks Public | TASK\_DEFAULTPUBLIC |
| Default New Phone Calls Public | CALL\_DEFAULTPUBLIC |
| Default Sync Category | DEFAULT\_CONTACT\_SYNC\_CATEGORY |
| **On the Alerts tab** |
| First Selection | EMAILALERT\_AM |
| Second Selection | EMAILALERT\_NOON |
| Third Selection | EMAILALERT\_PM |
| Include links in HTML alerts | LINKS\_EMAILALERT |
| Respect Quick Date Portlet Settings | USE\_QUICKDATE\_IN\_ALERTS |
| E-Mail | EMAILALERT\_EMAIL |
| Send an On-Demand Alert from this Role | ALERTONDEMAND |
| **On the Restrict View tab** |
| Subsidiary | SUBSIDIARY |
| Include Sub-Subsidiaries | SUBSIDIARYSUBS |
| Department | DEPARTMENT |
| Include Sub-Departments | DEPARTMENTSUBS |
| Include Unassigned | DEPARTMENTUNASSIGNED |
| Location | LOCATION |
| Include Sub-Locations | LOCATIONSUBS |
| Include Unassigned | LOCATIONUNASSIGNED |
| Class | CLASS |
| Include Sub-Classes | CLASSSUBS |
| Include Unassigned | CLASSUNASSIGNED |
| **On the Telephony tab** |
| Telephony Option | TELEPHONY\_OPTION |
| TAPI Device | TELEPHONYDEVICE |
| CTI URL | CTI\_URL |
| Prefix to Dial Out | DIALOUTPREFIX |

### Related Topics

-   [Permission Names and IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3236764.html)
-   [General Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3251492.html)
-   [Company Information Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3253690.html)
-   [Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3258805.html)
-   [Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3263666.html)
-   [Manufacturing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_160795960465.html)
-   [Tax Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N3263873.html)
-   [Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4695736720.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
