---
id: "chapter_N3361294"
type: "chapter"
title: "Suitelets and UI Object Best Practices"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Best Practices > Suitelets and UI Object Best Practices"
parent: "part_N3360914"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361294.html"
anchors: []
sha256: "2e381762567fa8c95b5dc1456b5bef188a95432b530eedc21df7521a628febfb"
---

The following are best practices for Suitelet development using UI objects and custom UI.

| General | 
-   Suitelets are ideal for generating NetSuite pages (forms, lists), returning data (XML, text), and redirecting requests.
-   Limit the number of UI objects on a page: less than 100 rows for sublists, less than 100 options for on demand select fields, and less than 200 rows for lists.

 |
| --- | --- |
| HTML | 

-   Try using inline HTML fields embedded on the form before implementing a full custom HTML page route.
-   Use Subresource Integrity when you include content from external sources in Inline HTML fields. For more information, see [Subresource Integrity](https://developer.mozilla.org/en-US/docs/Web/Security/Subresource_Integrity).

 |
| iFrames | 

-   Append 'ifrmcntnr=T' to the external URL when embedding in iFrame especially if you are using the Firefox browser. (For more about NetSuite and iFrame, see [Embedding an Online Form in your Website Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591690.html#bridgehead_N2592052).)

 |
| User credentials | 

-   When building a custom UI outside of the standard NetSuite UI (such as building a custom mobile page using Suitelet), use the [N/auth Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4296360422.html) and [N/crypto Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4358549582.html) to help users manage their credentials within the custom UI.

 |
| Calling a Suitelet and redirection | 

-   When calling a Suitelet using its external URL, escape the parameter values to avoid cross-site scripting injections, for example, by converting the appropriate characters to HTML entities.
-   For access or redirect to a Suitelet from another script, use [url.resolveDomain(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4861456597.html) to discover the URL instead of hard- coding the URL.

 |
| Advanced Employee Permissions | 

-   When the Advanced Employee Permissions feature is enabled, keep the following in mind:
    -   To avoid inadvertently exposing employee data, use caution when running Suitelets or Restlets as an administrator. A user with a role that has limited access to the employee record can access a Suitelet or Restlet that runs as an administrator. Depending on how the Suitelet or Restlet is written, the user may have access to employee information that they would otherwise not see.
    -   Use caution when setting up Suitelets and Restlets to give access to users without having to log in since it could potentially expose employee information in uncontrolled ways.

 |
| Deployment | 

-   Deploy Suitelets as 'Available without Login' only if necessary (no user context, login performance overhead). (See [Setting Available Without Login](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2997713.html).)

 |

### Related Support Articles

-   [SuiteApp Architectural Fundamentals and Examples (SAFE Guide)](https://suiteanswers.custhelp.com/ci/okcsFattach/getFile/1011960/SuiteAppArchitecturalFundamentalsandExamples.pdf)

### Related Topics

-   [SuiteScript Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/part_N3360914.html)
-   [General Development Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361037.html)
-   [Client Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361924.html)
-   [Map/Reduce Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0801064715.html)
-   [Scheduled Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361671.html)
-   [User Event Script Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3361453.html)
-   [Optimizing SuiteScript Performance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460387617.html)
-   [SuiteScript Security Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_159804448843.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
