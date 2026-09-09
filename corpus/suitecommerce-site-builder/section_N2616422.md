---
id: "section_N2616422"
type: "section"
title: "Using Attribute Tags in Site Templates"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Creating Attribute Tags > Using Attribute Tags in Site Templates"
parent: "section_N2615537"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616422.html"
anchors: []
sha256: "a450eb815b82df809903cbbc38acbf13dd49d8b7feaaa79ea36a904126f61b98"
---

You can use Attribute tags for customizing HTML templates for use on your website. This lets you control the look and feel of your site. You decide where to display images and how to display information from NetSuite records on your website. Note that Web Site Tags are not supported in SuiteCommerce Advanced.

For more information about options for customizing your website with Attribute tags, see [Customizing Site Themes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603752.html) and [Item and Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606158.html).

The code sample below is from an item/category template for the related items list.

          `<TABLE border=0 cellspacing=0 cellpadding=0 width="100%">    <TR>       <TD valign="top"><b><%=getCurrentAttribute('item', 'relatedItemsDescription')%></b></TD>    </TR>    <TR>        <TD valign="top"><a href="https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/<%=getCurrentAttribute('item','storeurl')%>"; onMouseover="this.className='lnk13b-blackOn'; return true;" onMouseout="this.className='lnk13b-blackOff'; return true;"><%=getCurrentAttribute('item','storedisplayname2')%></a></TD>    </TR>    <TR>       <TD valign="top"><STRONG><%=getCurrentAttribute('item','stockstatusmessagehtml')%></STRONG></TD>    </TR>    <TR>        <TD valign="top"><%=getCurrentAttribute('item','storedescription2')%></TD>    </TR>    <TR>       <TD><IMG src="https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/images/common/spacer.gif" width=1 height=5></TD>           </TR>    <TR><TD bgcolor="#CCCCCC"><IMG src="https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/images/common/spacer.gif" width=1 height=1></TD>    </TR>    <TR><TD><IMG src="https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/images/common/spacer.gif" width=1 height=5></TD></TR> </TABLE>` 
        

### Related Topics

-   [Using Web Site Tags in Hosted Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616592.html)
-   [Creating Attribute Tags for Custom Records and Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616759.html)
-   [Creating Attribute Tags for Standard Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html)
-   [Creating Attribute Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615537.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
