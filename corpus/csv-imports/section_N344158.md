---
id: "section_N344158"
type: "section"
title: "Choose Import Character Encoding"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Step One Scan & Upload File > Choose Import Character Encoding"
parent: "section_N343532"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html"
anchors: []
sha256: "ec3b0dd2173bc90b5101d5697f0159fdfcf433dd40823767e9b04d1a8b0fcf27"
---

On the Scan & Upload File page, choose the character encoding for your CSV import. The one you choose depends on the type of file you're importing.

Encoding schemes generally act the same way for common characters, such as 'a', 'A', and '0'. For special characters that programs may generate automatically as you type, such as typographic quotation marks, and for characters with diacriticals, encoding schemes differ, for example 0xE9 vs. 0x8E for 'e' + acute accent.

NetSuite supports the following types of character encoding:

-   **(Unicode) UTF-8 encoding** - UTF-8 character encoding is the most widely used format for international users importing a CSV file created in a language other than U.S. English.
    
    If you want to use this format, make sure your file has valid UTF-8 characters. You might need a third-party editor to convert your file to UTF-8 before importing it into NetSuite. Some editors add a BOM (Byte Order Marker) at the beginning of the file to show it's UTF-8 encoded, but NetSuite will import UTF-8 files whether the BOM is there or not.
    
    On Windows, you can use Notepad to convert your CSV to UTF-8. Open your file in Notepad, go to File > Save As, select UTF-8 from the Encoding dropdown, and click Save.
    
-   **Western (Windows 1252) encoding** - Typically, NetSuite users create CSV files for import in Microsoft Excel, which uses Windows 1252 character coding. Western (Windows 1252) is the default for the U.S. edition.
    
-   **Western (ISO-8859-1) encoding** - ISO-8859-1 encodes what is commonly referred to as 'Latin alphabet no. 1,' consisting of 191 characters from the Latin script. The character-encoding is used throughout the Americas, Western Europe, Oceania, and much of Africa. It is also commonly used in most standard romanizations of East Asian languages.
    
-   **Chinese Simplified (GB18030)** - GB18030 is the registered Internet name for the official character set of the People's Republic of China (PRC), superseding GB2312. The character set is formally called 'Chinese National Standard GB 18030-2005: Information technology -- Chinese coded character set.' GB abbreviates Guójiā Biāozhun, which means national standard in Chinese. (Description cited from Wikipedia.) Chinese Simplified (GB18030) is the default if you select the Chinese language preference.
    
-   **Chinese Simplified (GBK) encoding extension** - Used in mainland China and Singapore.
    
-   **Traditional Chinese (Big5) encoding** - Typically used in Taiwan (Province of China), Hong Kong, and Macao.
    
-   **Japanese (Shift-JIS) encoding** - Shift-JIS character encoding is the most widely used format for Japanese users importing a CSV file. Japanese (Shift-JIS) is the default for the Japanese edition and when you select the Japanese language preference.
    
-   **(Western) MacRoman** - CSV files created in Excel running on Macs use MacRoman character encoding.
    
-   **Korean (ISO-2022-KR) encoding** - Character code structure for Korean text (ISO standard).
    
-   **Korean (EUC-KR) encoding** - One of the more widely-used legacy character encodings (extended UNIX code).
    

Note:

If invalid characters prevent a file from being processed for import, you receive an error and can fix it. For more information, see [CSV Import Error Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353446.html).

### Related Topics

-   [Step One Scan & Upload File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N343532.html)
-   [Select an Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N343713.html)
-   [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html)
-   [Choose CSV Column Delimiter](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4341195935.html)
-   [Select a File for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344348.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
