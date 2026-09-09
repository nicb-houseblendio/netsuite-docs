---
id: "section_N492354"
type: "section"
title: "Words Excluded from Duplicate Detection Matching"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Duplicate Record Detection > Words Excluded from Duplicate Detection Matching"
parent: "section_N490932"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N492354.html"
anchors: ["bridgehead_N492373", "bridgehead_N492448", "bridgehead_N492721", "bridgehead_N492732"]
sha256: "d45da0af2633306ab470d7c44e0b32c3bc031c322d8acdc6b2fbfc99a9840ee5"
---

Records are listed as duplicates when they have either matching or similar information. When searching for similar information, NetSuite excludes certain words or phrases that occur often in fields to avoid false duplicates. This list is organized by field name.

## Customer, Partner, and Vendor Name {#bridgehead_N492373}

The following words or abbreviations aren't considered when searching for similar information to prevent false matches in the company or customer name field:

-   Corp.
    
-   Corporation
    
-   Co.
    
-   Company
    
-   Inc.
    
-   Incorporated
    
-   Enterprise(s)
    
-   Firm
    

Note that duplication detection also ignores variations of these terms, such as abbreviations without periods at the end.

## Email Address {#bridgehead_N492448}

If you identify duplicates based on matching email address, you can set duplicate criteria on **Email (full)** to identify duplicates only if the full email addresses of two records match exactly.

If you set duplicate criteria based on **Email (domain only)**, the domain names listed below aren't considered when searching for similar information to prevent false matches for email addresses. Administrators can add or remove a domain from the default list in the Excluded Domains subtab on the Set Up Duplicate Detection page at _Setup > Company > Company Management > Duplicate Detection_. Administrators can also configure a unique list of domains to be excluded from Email (domain only).

-   adelphia.net
    
-   altavista.com
    
-   ameritech.net
    
-   aol.com
    
-   attbi.net
    
-   att.net
    
-   bellsouth.net
    
-   bigfoot.com
    
-   comcast.net
    
-   cox.net
    
-   earthlink.com
    
-   excite.com
    
-   gmail.com
    
-   home.com
    
-   hotmail.com
    
-   ix.netcom.com
    
-   juno.com
    
-   lycos.com
    
-   mindspring.com
    
-   msn.com
    
-   netscape.net
    
-   netzero.com
    
-   pacbell.net
    
-   prodigy.net
    
-   qwest.net
    
-   sbcglobal.net
    
-   swbell.net
    
-   sympatico.ca
    
-   verizon.net
    
-   worldnet.att.net
    
-   yahoo.com
    
-   yahoo.co.uk
    

Note:

Potential duplicate results are determined differently when using the email address from a customer record than from a contact record. Customer records are flagged as potential duplicates when the domain name portion of the address matches, provided the domain name isn't listed on the Excluded Domains list. Contact records are flagged as duplicates only if the entire email address matches. This difference prevents false potential duplicate results when multiple contact records from one company use the same domain name in their email addresses.

## Phone Number {#bridgehead_N492721}

When searching the phone number field for duplicates, all prefixes and extensions are excluded so that only the 9 digit or 6 digit numbers are considered. If you compare two matching phone numbers, but one has an area code and the other doesn't, they won't be detected as duplicates.

## Address {#bridgehead_N492732}

Addresses are considered potential duplicates based on the street number and name. Similar numbers with a street name match are considered potential duplicates, for example.

The following words or symbols aren't considered when searching for potential duplicates in the Address field:

-   Street/St.
    
-   Avenue/Ave.
    
-   Court/Ct.
    
-   Suite/Ste.
    
-   Apartment/Apt.
    
-   #
    
-   Lane/Ln.
    
-   Highway/Hwy.
    
-   Road/Rd.
    
-   West/W.
    
-   North/N.
    
-   East/E.
    
-   South/S.
    
-   NW
    
-   SW
    
-   SE
    

### Related Topics

-   [Duplicate Record Detection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N490932.html)
-   [Merging or Deleting Duplicate Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N491111.html)
-   [Merging Large Numbers of Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3744355188.html)
-   [Merging Different Types of Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N491887.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
