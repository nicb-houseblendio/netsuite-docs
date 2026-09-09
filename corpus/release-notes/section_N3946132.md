---
id: "section_N3946132"
type: "section"
title: "SuiteApp Distribution"
branch: "release-notes"
category: "what-s-new"
breadcrumb: "What's New > Release Notes > NetSuite 2026.2 Release Notes > SuiteApp Distribution"
parent: "article_72152418635"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3946132.html"
anchors: ["subsect_0529102722"]
sha256: "bb5df299d950375f4f680f368216988993188cafd3ad2ff03d941b42bcfa5bb1"
---

SuiteApp distribution includes SuiteBundler, SuiteApp Marketplace, and SuiteApp Control Center capabilities that you can use to distribute customizations to accounts.

NetSuite 2026.2 includes the following enhancements to SuiteApp distribution features:

## New SuiteApp Control Center REST API Endpoints for Publishing, Upgrading, and Deprecating SuiteApps {#subsect_0529102722}

SuiteApp Control Center REST API now provides more ways to automate SuiteApp lifecycle management. You can now publish or deprecate SuiteApp versions, upgrade SuiteApp installations, and retrieve installations by managed upgrade eligibility and upgrade phase.

Use the new `PATCH` endpoint to publish a pending SuiteApp version or deprecate a released SuiteApp version. Use the new `PUT` endpoint to upgrade SuiteApp installations to a selected SuiteApp version.

The `GET` endpoint now includes new query parameters that return only installations eligible for managed upgrade. You can filter results by upgrade phase, such as leading or lagging. If you do not specify an upgrade phase, the endpoint uses the leading upgrade phase by default.

To use these endpoints, you must use the Release Manager role. For more information, see [Getting Started with SuiteApp Control Center REST API Endpoints](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0105013037.html).

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
