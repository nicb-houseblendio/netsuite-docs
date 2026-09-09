---
id: "bridgehead_N2881626"
type: "bridgehead"
title: "The Icon Sprite Image File for Custom Records"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Records Overview > Creating Custom Record Types > Choosing an Icon for a Custom Record > Creating Icons for Custom Records > The Icon Sprite Image File for Custom Records"
parent: "section_N2881458"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2881626.html"
anchors: []
sha256: "0ad59f8b4b74535442892a80ee67542ce58f36d60d856688dfc60c5ff2f0e21e"
---

This topic describes the icon sprite image file for creating custom icons. For information about the four icon versions, see [The Four Icon Versions for Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2881553.html) For an overview of general requirements and file specifications, see [Creating Icons for Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2881458.html).

The four icon versions reside, side-by-side, in a single image file known as a sprite. Using coordinates and other data stored in CSS, NetSuite displays the proper icon version needed and crops out and hides the rest of the sprite image. Therefore, for your icons to display properly, they must be an exact size and at an exact location within the image file.

Each icon must be no larger than 16 pixels by 16 pixels. Any artwork that goes beyond the 16x16 boundary will not be displayed.

![Sample Icon Sprite Image file.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/CR_Icons_spriteimage_01.png)

Each icon version must be located at the following locations within the image file, as measured from the upper-left corner of the image:

| Icon Version | x Coordinate | y Coordinate |
| --- | --- | --- |
| Grayscale icon for dark backgrounds | 25 | 25 |
| Grayscale icon for light backgrounds | 50 | 25 |
| Color icon for dark backgrounds | 75 | 25 |
| Color icon for light backgrounds | 100 | 25 |

Most image-editing applications have guides that you can set up to help you keep track of these spacing requirements. You can also download the sample icon file pack at the bottom of this topic, which contains various template files that will help keep your icons in order.

### Related Topics

-   [Creating Icons for Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2881458.html)
-   [The Four Icon Versions for Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2881553.html)
-   [File Format for Custom Record Icons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2881880.html)
-   [Constructing Your Custom Record Icon File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1117120409.html)
-   [Sample Icons for Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2882057.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
