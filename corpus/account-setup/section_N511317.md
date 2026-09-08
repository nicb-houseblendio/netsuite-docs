---
id: "section_N511317"
type: "section"
title: "Setting Up TAPI Telephony Integration"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Company Settings > Using Telephony Integration > Setting Up TAPI Telephony Integration"
parent: "section_N511129"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N511317.html"
anchors: ["procedure_N511347"]
sha256: "6b64fa631bf1929c5e3d64d2017c7e187ab2c5d99d0680df7245e29a957f79c5"
---

Telephony Application Programming Interface (TAPI) must be set up on each user's PC. You must have a TAPI compliant phone and software. TAPI integration requires the ActiveX component which is only available in the Internet Explorer browser.

To set up TAPI integration, the account administrator must first enable the Telephony Integration feature at _Home > Set Preferences_ on the Telephony subtab. After downloading the driver, enter the name of the TAPI enabled phone.

Note:

Two versions of TAPI are available, TAPI 2.x and TAPI 3.x. NetSuite supports both TAPI versions.

#### To set up telephony integration with a TAPI device: {#procedure_N511347}

1.  Go to _Home > Set Preferences_.
    
2.  On the **Telephony** subtab, in the **Telephony Option** field, select **TAPI Device**.
    
3.  Follow the on-screen instructions to download the `ExceleTelforNetSuiteApplications.zip` file, which contains the executable file needed to install the required drivers for Telephony Integration.
    
    ![Telephony subtab with download instructions.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/AccountSetup/SetPreferences_TelephonyTAPI.png)
4.  In the **TAPI Device** field, enter the device that controls communication with your phone. If you do not know the name of your TAPI device, you can use a sample program at [www.exceletel.com](https://www.exceletel.com/sandbox/samples) to find this information.
    
5.  In the **Prefix to Dial Out** field, enter any numbers that must be dialed before dialing a phone number in your phone system. For example, you may need to dial 9 or 1 before a number.
    
6.  Click **Save**.
    

If you have trouble locating the name of your TAPI device or receive an error message that it could not be found, try the following troubleshooting tips:

-   If the name of your TAPI device ends with extension.tsp, try leaving out this extension when entering the name in NetSuite.
    
-   The TAPI Device field is case-sensitive and must match your device name exactly.
    
-   Download a sample program [here](https://www.exceletel.com/sandbox/samples) to test dialing from your phone. From the exceletel Web page, click **etQuickDial** to download the etQuickDial program.
    
    When the program has downloaded, open the program and view all TAPI-enabled devices on your computer in the Active field. Select the device you are using, and check the Active box. Then enter a phone number to dial and click Dial to make sure the call is initiated from your device correctly.
    

To learn how to initiate and end calls, see [Making Calls From NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N511709.html).

### Related Topics

-   [Using Telephony Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N511129.html)
-   [Setting Up CTI Telephony Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N511458.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
