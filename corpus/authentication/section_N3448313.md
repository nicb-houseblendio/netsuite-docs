---
id: "section_N3448313"
type: "section"
title: "PCI Compliance Password Requirements"
branch: "authentication"
category: "account-administration"
breadcrumb: "Account Administration > Authentication > Password Requirements and Policies in NetSuite > PCI Compliance Password Requirements"
parent: "chapter_4713604654"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3448313.html"
anchors: []
sha256: "9473fb9f4d267abc69e00dead564e9288e3308e3e1a87c5a1d411f734d5d26a2"
---

NetSuite abides Payment Card Industry Data Security Standard (PCI DSS) password requirements. Users with either the View Unencrypted Credit Cards permission or the View Unencrypted ACH Account Numbers permission must change their passwords at least every 90 days.

If the number of days set in the **Password Expiration in Days** field on the General Preferences page is less than 90 days, the company requirement remains in effect. For example, if a company is set to expire passwords every 60 days, your password expiration date doesn't change. However, if the company is set to expire passwords every 120 days, this setting automatically changes to 90 days for users with either the View Unencrypted Credit Cards permission or the View Unencrypted ACH Account Numbers permission.

Passwords for users with access to unencrypted credit card numbers or unencrypted ACH accounts must have a minimum of 12 characters. If the number of characters set in the **Minimum Password Length** field on the General Preferences page is greater, that greater requirement remains in effect.

All users with access to unencrypted credit card numbers or unencrypted ACH accounts must change passwords to comply with the PCI requirements.

### Related Topics

-   [Password Requirements and Policies in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4713604654.html)
-   [NetSuite Password Requirements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N250541.html)
-   [User Access Reset Tool](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156442554498.html)
-   [Password Reset Tips for Administrators](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1512656886.html)
-   [Password Changes Are Logged in System Notes on Entity Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156587964668.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
