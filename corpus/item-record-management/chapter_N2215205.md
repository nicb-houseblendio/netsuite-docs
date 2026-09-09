---
id: "chapter_N2215205"
type: "chapter"
title: "Bar Codes and Item Labels"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Bar Codes and Item Labels"
parent: "book_N2164398"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2215205.html"
anchors: []
sha256: "bc05cf0a31c31c51172a4ac3896109f64b8f54a594b1a4faedeed4ea36d6f872"
---

The Bar Coding and Item Labels feature automatically generates a bar code for each item. This bar code is based on the Item Name/Number, or Stock Keeping Unit (SKU), on the item record. Item bar codes are generated based on the contents of the Item Name/Number field in an item record. Most bar codes use a number or alphanumeric string for this field.

Bar codes are also generated for each transaction, as well as serial numbers if you use them.

The NetSuite bar code integration works with any bar code scanner that functions as a keyboard input device. The scanner translates the bar code into text, as if you typed it on the keyboard.

You can input and track information in NetSuite by generating bar codes for each item and transaction. For example, you can:

-   Print labels to affix to the items that show the item price, and bar codes for item number and serial number.
    
-   Scan bar code labeled items to add them to a sales transaction or receive them on a purchase transaction.
    
-   Scan transaction bar codes to bulk receive, fulfill, pick, pack, ship, bill, or approve orders.
    

Bar codes for items can be generated in one of the following formats:

-   **UPC** - specific number of integer characters
    
    A UPC bar code symbol is a pattern of black bars with white spaces with numbers below. The numbers are encoded in the symbol and uniquely identify the product. This group of numbers is referred to as a Global Trade Item Number (GTIN). Scanners read the symbol to capture the GTIN, which computer systems then use to track sales and product orders. The GTIN in a UPC Bar Code Symbol is always 12-digits in length.
    
    Note:
    
    A 12-digit UPC code will have the country digit appended as the first digit. The country digit for the US is 0.
    
    For more information, see [http://www.uc-council.org](http://www.uc-council.org/)
    
-   **EAN** - bar codes that have 13-digits are EAN format
    
-   **Code 128** - allows alphanumeric and non-printing characters
    
    Code 128 is a very high density alphanumeric bar code, and is more flexible than the UPC format. The symbol can be as long as necessary to store the encoded data. It's designed to encode text, numbers, several functions and the entire 128 character ASCII character set.
    
    For more information, see [http://www.idautomation.com/barcode-faq/code-128/](http://www.adams1.com/128code.html)
    

You can indicate which bar code format you are using on a per item basis.

### Related Topics

-   [Using Code 128 Bar Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163292085605.html)
-   [Enabling the Advanced Inventory Management Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162488513759.html)
-   [Enabling the Bar Coding and Item Labels Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163292087805.html)
-   [Printing Bar Code and Item Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2215536.html)
-   [Scanning Bar Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2218627.html)
-   [Processing Orders Using Bar Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N561778.html)
-   [Printing Labels From Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N562976.html)
-   [Using Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2164525.html)
-   [Item Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2180614.html)
-   [Item Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2191369.html)
-   [Multiple Units of Measure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2211898.html)
-   [Item Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2222944.html)
-   [Customer Part Number](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4575965810.html)
-   [Effective Date Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1536354469.html)
-   [Item Record Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N2164398.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
