---
id: "section_N3386227"
type: "section"
title: "Moving a Bundle Out of the Bundle Repository"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Saved Bundles > Bundle Availability > Moving a Bundle Out of the Bundle Repository"
parent: "section_N3385668"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3386227.html"
anchors: ["svg_1", "svg_1background", "svg_1Arrows", "svg_1Shapes_and_text", "svg_1Node_2_", "svg_1Callouts"]
sha256: "568d9bdfb7dfa6d0fe386893a908a5ac9343327c0d05921745f10f230d699812"
---

Important:

The NetSuite bundle repository was deprecated as of January 18, 2021.

If you have not already done so, take the required actions shown in the following diagram to remove your existing bundles from the bundle repository. There are five possible scenarios for bundles in the repository that may require you to take action. These different scenarios are indicated by the numbers in the diagram.

<a id="svg_1"></a>

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         

Based on your chosen use case in the preceding diagram, see the following options for moving your bundles out of the repository:

-   **Scenario 1:** You need to continue upgrades to the bundle install base, and you have access to the bundle source account and to a secondary account.
    
    1.  Copy a bundle to a secondary account and deprecate the bundle stored in the repository.
        
        See [Remove Install Base of Custom Bundle Out of NetSuite Repository](https://suiteanswers.custhelp.com/app/answers/detail/a_id/90588).
        
    2.  After deprecating the bundle stored in the repository with the bundle copied to the secondary account, the bundle from the secondary account will be the one installed into target accounts, instead of the bundle from the repository.
        
    3.  After this deprecation, the bundle from the secondary account will be the one installed into target accounts, instead of the bundle from the repository.
        
-   **Scenario 2:** You need to continue upgrades to the bundle install base and you do not have access to the bundle source account.
    
    1.  File a case with NetSuite Support to gain access to the source account for the bundle.
        
    2.  Start the case title with the following prefix: Bundle repository deprecation support
        
    3.  Include the bundle ID and account ID of the bundle source account that you cannot access.
        
    4.  After you gain access to this source account, check whether you have access to a secondary account. If yes, see Scenario 1. If no, see Scenario 3.
        
-   **Scenario 3:** You need to continue upgrades to the bundle install base, you have access to the bundle source account, but not to a secondary account.
    
    1.  To purchase an additional account, please contact your Account Manager or Sales Rep.
        
    2.  If you do not know your Account Manager, please contact NetSuite Customer Support and ask for this information.
        
    3.  After you have purchased an additional account, see Scenario 1.
        
-   **Scenario 4:** You do not need to continue upgrades to the bundle install base, but you want to keep the bundle objects and you have access to the bundle source account.
    
    You have the option of making the bundle available for future tasks in SDF instead of SuiteBundler. To convert a bundle into an SDF account customization project, see [Converting a Bundle into an Account Customization Project from a NetSuite Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1562952652.html).
    
    Note:
    
    Converting a bundle into an account customization project saves the bundle definition as a zip file in the file cabinet.
    
-   **Scenario 5:** You do not need to continue upgrades to the bundle install base, but you want to keep the bundle objects and you do not have access to the bundle source account.
    
    1.  You can install the bundle in a different account so that you will have access to the bundle objects in the future. To install a bundle in your new account, see [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html).
        
        Note:
        
        If a bundle installed in a new account contains locked objects, you can file a support issue to get these locked objects unlocked.
        
    2.  After the bundle is in a new account that you can access, you have the option to convert the bundle into an SDF account customization project. See Scenario 4.
        

### Related Topics

-   [Bundle Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385668.html)
-   [Sharing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3385867.html)
-   [Deprecating a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3386679.html)
-   [Implementing Phased Updates by Setting Bundle Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3387345.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
