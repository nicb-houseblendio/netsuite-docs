---
id: "section_N404433"
type: "section"
title: "Common Errors When Importing Routing Records"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Supply Chain Import Type > Manufacturing Routing Import > Common Errors When Importing Routing Records"
parent: "section_N399906"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N404433.html"
anchors: ["bridgehead_N404445", "bridgehead_3705045937", "bridgehead_N404499", "bridgehead_N404516"]
sha256: "ec9cfc1547bff0e52376401ed9888ab3099cd32cf525b00d284454740ed75985"
---

The 'Results' file for a failed routing record import might include any of the following messages.

## You must enter at least one line {#bridgehead_N404445}

This error indicates that you failed to include sublist data for every routing record. Each routing record must have at least one sublist record.

If you're doing a multiple-file import, this error might point to a problem with the key column you're using to link the files. For example, one of the files might include a typo in this column, preventing proper linking of the routing record body data to its sublist data.

## Invalid location reference key {#bridgehead_3705045937}

This error could indicate that any of the following occurred:

-   You entered an incorrect value for the Location field. For example, you might have included a typo in the location name.
    
-   You entered a location that is not valid for the subsidiary being referenced.
    
-   You entered multiple valid locations but made a formatting error. For example, if you placed spaces around the Multi-Select Value Delimiter (the default is a |), the system generates this error.
    

## This sequence number is already in use on another step {#bridgehead_N404499}

Indicates that you mapped a value to the Operation Sequence field that is not unique for the routing record being referenced. For example, you entered two operations with the sequence '20.'

If you're doing a multiple-file import, this error might point to a mistake with the unique identifier used to link the sublist records to the body data. For example, suppose your file defines Routings A and B, each of which includes three operations with sequence values of 10, 20, and 30. If you inadvertently associated one of the Routing B rows with the same unique identifier used for Routing A, then you would get this error.

## 'Invalid manufacturingworkcenter reference key Value' {#bridgehead_N404516}

Indicates that you mapped an invalid value to the Manufacturing Work Center field. If you're certain you entered the correct name of an employee group, check to make sure that the record for the group has the Manufacturing Work Center box selected.

### Related Topics

-   [Manufacturing Routing Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N399906.html)
-   [Prerequisite Records for Routing Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N400118.html)
-   [Routing Body and Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N400811.html)
-   [Routing CSV File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N401643.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
