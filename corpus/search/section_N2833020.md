---
id: "section_N2833020"
type: "section"
title: "SQL Expressions"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Formulas in Searches > SQL Expressions"
parent: "article_5143710889"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html"
anchors: ["bridgehead_4431020844", "bridgehead_N2833224", "bridgehead_N2834645", "bridgehead_N2835588", "bridgehead_N2836025", "bridgehead_N2836356", "bridgehead_N2836578", "bridgehead_N2836722", "bridgehead_N2839038", "bridgehead_N2839271"]
sha256: "27527c4446d24facdd59f80522ed41a5405b0a69f479c0fb30dfbb563f75c30a"
---

The SQL expressions that you enter in field formulas call the Oracle database to evaluate the function, and those functions are maintained by Oracle. For more information about these functions, see the [Oracle Database SQL Reference](https://docs.oracle.com/en/database/oracle/oracle-database/23/sqlqr/index.html).

Important:

The following material is provided for convenience only. It is assumed that you are familiar with the implementation of SQL expressions. For a complete reference to SQL expressions, [go to the Oracle website](https://docs.oracle.com/en/database/oracle/oracle-database/18/sqlqr/SQL-Expressions.html#GUID-70883820-21B4-440C-8563-84AF1DBA1FE2) (requires Oracle account activation). Not all of the expressions described at the URL are supported in NetSuite.

If you are familiar with Microsoft SQL Server functions but are new to Oracle databases, see [Character Functions](https://docs.oracle.com/cd/E10405_01/appdev.120/e10379/ss_oracle_compared.htm#i1038077) to compare SQL functions support in Microsoft SQL Server and Oracle databases. If you are used to Microsoft Excel functions, please note that not all Excel functions are supported by Oracle, and those that are supported often use a different syntax.

The following tables outline the SQL functions that can be used in NetSuite search formulas and custom formula fields:

-   [Numeric Functions](#bridgehead_N2833224)
    
-   [Character Functions Returning Character Values](#bridgehead_N2834645)
    
-   [Character Functions Returning Number Values](#bridgehead_N2835588)
    
-   [Datetime Functions](#bridgehead_N2836025)
    
-   [NULL-Related Functions](#bridgehead_N2836356)
    
-   [Decode](#bridgehead_N2836578)
    
-   [Sysdate](#bridgehead_N2836722)
    
-   [Case](#bridgehead_N2839038)
    
-   [Analytic and Aggregate Functions](#bridgehead_N2839271)
    

Important:

To avoid cross-scripting (XSS) vulnerabilities, search column results with formulas that contain <script> tags do not display script output. Do not use <script> tags in your search formulas.

Note:

You cannot combine aggregate and non-aggregate SQL functions in the same formula definition. For example, if you create a formula using an aggregate function, then all the functions in the definition must either be aggregate functions or listed in a GROUP\_BY clause.

## Conventions in SQL Syntax Examples {#bridgehead_4431020844}

The syntax examples use [Oracle's typographic conventions for SQL code examples](http://docs.oracle.com/cd/B19306_01/appdev.102/b14261/preface.htm#i970948). The following table shows the conventions used in SQL syntax examples.

| Convention | Meaning | Example |
| --- | --- | --- |
| \[ \] | Anything enclosed in brackets is optional. | LTRIM(char \[ , set \]) |
| { } | Braces are used for grouping items. | TO\_CHAR({ datetime | interval } \[, fmt \[, 'nlsparam' \] \]) |
| | | A vertical bar represents a choice of two options. | ATAN2(n1 { , | / } n2) |
| ... | An ellipsis mean repetition in syntax descriptions or an omission in code examples or text. | DECODE(expr, search, result \[, search, result \]...\[, default \]) |
| UPPERCASE | Indicates an element supplied by the system. These terms are shown in uppercase to distinguish them from terms you define. Unless terms appear in brackets, enter them in the order and with the spelling shown. Because these terms are not case sensitive, you can use them in either UPPERCASE or lowercase. | TRIM(\[ { { LEADING | TRAILING | BOTH }\[ trim\_character \] | trim\_character } FROM \] trim\_source) |
| lowercase | Indicates user-defined programmatic elements, such as field names. Note that some programmatic elements use a mixture of UPPERCASE and lowercase. Enter these elements as shown. | NULLIF(expr1, expr2) |

The examples are provided for illustrative purposes only. They may or may not work for you, depending on your NetSuite account settings and data.

## Numeric Functions {#bridgehead_N2833224}

| Function | Syntax | Description | Example |
| --- | --- | --- | --- |
| ABS | ABS(n) | returns the absolute value of n | ABS({amount}) |
| ACOS | ACOS(n) | returns the arc cosine of n | ACOS(0.35) |
| ASIN | ASIN(n) | returns the arc sine of n | ASIN(1) |
| ATAN | ATAN(n) | returns the arc tangent of n | ATAN(0.2) |
| ATAN2 | ATAN2(n1 { , | / } n2) | returns the arc tangent of n1 and n2 | ATAN2(0.2, 0.3) |
| BITAND | BITAND(expr1, expr2) | computes an AND operation on the bits of expr1 and expr2 | BITAND(5, 3) |
| CEIL | CEIL(n) | returns smallest integer greater than or equal to n | CEIL({today}-{createddate}) |
| COS | COS(n) | returns the cosine of n | COS(0.35) |
| COSH | COSH(n) | returns the hyperbolic cosine of n | COSH(-3.15) |
| EXP | EXP(n) | returns e raised to the nth power, where e = 2.71828183 | EXP({rate}) |
| FLOOR | FLOOR(n) | returns largest integer equal to or less than n | FLOOR({today}-{createddate}) |
| LN | LN(n) | returns the natural logarithm of n | LN(20) |
| LOG | LOG(n2, n1) | returns the logarithm, base n2, of n1 | LOG(10, 20) |
| MOD | MOD(n2, n1) | returns the remainder of n2 divided by n1 | MOD({today}-{lastmessagedate},7) |
| NANVL | NANVL(n2, n1) | returns an alternative value n1 if the input value n2 is not a number | NANVL({itemisbn13}, '') |
| POWER | POWER(n2, n1) | returns n2 raised to the n1 power | POWER({custcoldaystoship},-.196) |
| REMAINDER | REMAINDER(n2, n1) | returns the remainder of n2 divided by n1 | REMAINDER({transaction.totalamount}, {transaction.amountpaid}) |
| ROUND (number) | ROUND(n \[, integer \]) | returns n rounded to integer places to the right of the decimal point | ROUND(({today}-{startdate}), 0) |
| SIGN | SIGN(n) | returns the sign of n | SIGN({quantity}) |
| SIN | SIN(n) | returns the sine of n | SIN(5.2) |
| SINH | SINH(n) | returns the hyperbolic sine of n | SINH(3) |
| SQRT | SQRT(n) | returns the square root of n | SQRT(POWER({taxamount}, 2)) |
| TAN | TAN(n) | returns the tangent of n | TAN(-5.2) |
| TANH | TANH(n) | returns the hyperbolic tangent of n | TANH(3) |
| TRUNC (number) | TRUNC(n1 \[, n2 \]) | returns n1 truncated to n2 decimal places | TRUNC({amount}, 1) |

## Character Functions Returning Character Values {#bridgehead_N2834645}

| Function | Syntax | Description | Example |
| --- | --- | --- | --- |
| CHR | CHR(n \[ USING NCHAR\_CS \]) | returns the character having the binary equivalent to n as a VARCHAR2 value | CHR(13) |
| CONCAT | CONCAT(char1, char2) | concatenates char1 and char2 into one string | CONCAT({number},CONCAT('\_',{line})) |
| INITCAP | INITCAP(char) | returns char, with the first letter of each word in uppercase, all other letters in lowercase | INITCAP({customer.companyname}) |
| LOWER | LOWER(char) | returns char, with all letters lowercase | LOWER({customer.companyname}) |
| LPAD | LPAD(expr1, n \[, expr2 \]) | returns expr1, left-padded to length n characters with the sequence of characters in expr2 | LPAD({line},3,'0') |
| LTRIM | LTRIM(char \[, set \]) | removes from the left end of char all of the characters contained in set | LTRIM({companyname},'-') |
| REGEXP\_REPLACE | 
REGEXP\_REPLACE(source\_char, pattern

\[, replace\_string

\[, position

\[, occurrence

\[, match\_parameter \]

\]

\]

\]

)



 | lets you replace a sequence of characters (source\_char) that matches a regular expression pattern with another set of characters (replace\_string) | REGEXP\_REPLACE({name}, '^.\*:', '') |
| REGEXP\_SUBSTR | 

REGEXP\_SUBSTR(source\_char, pattern

\[, position

\[, occurrence

\[, match\_parameter \]

\]

\]

)



 | lets you extract a sequence of characters that matches a regular expression pattern from the source string (source\_char) | REGEXP\_SUBSTR({item},'\[^:\]+$') |
| REPLACE | 

REPLACE(char, search\_string

\[, replacement\_string \]

)



 | returns char with every occurrence of search\_string replaced with replacement\_string | REPLACE({serialnumber}, '&', ',') |
| RPAD | RPAD(expr1 , n \[, expr2 \]) | returns expr1, right-padded to length n characters with expr2, replicated as many times as necessary | RPAD({firstname},20) |
| RTRIM | RTRIM(char \[, set \]) | removes from the right end of char all of the characters that appear in set | RTRIM({paidtransaction.externalid},'-Invoice') |
| SOUNDEX | SOUNDEX(char) | returns a character string containing the phonetic representation of char | SOUNDEX({companyname}) |
| SUBSTR | 

SUBSTR(char, position \[, substring\_length \])



 | returns a portion of char, beginning at character position, substring\_length characters long | SUBSTR({transaction.salesrep},1,3) |
| TRANSLATE | TRANSLATE(expr, from\_string, to\_string) | returns expr with all occurrences of each character in from\_string replaced by its corresponding character in to\_string | TRANSLATE({expensecategory}, ' ', '+') |
| TRIM | 

TRIM(\[ { { LEADING | TRAILING | BOTH }

\[ trim\_character \]

| trim\_character

}

FROM

\]

trim\_source

)



 | lets you trim leading or trailing characters (or both) from a character string | TRIM (BOTH ',' FROM {custrecord\_assetcost}) |
| UPPER | UPPER(char) | returns char, with all letters uppercase | UPPER({unit}) |

## Character Functions Returning Number Values {#bridgehead_N2835588}

| Function | Syntax | Short Description | Example |
| --- | --- | --- | --- |
| ASCII | ASCII(char) | returns the decimal representation in the database character set of the first character of char | ASCII({taxitem}) |
| INSTR | 
INSTR(string , substring

\[, position

\[, occurrence \]

\])



 | searches string for substring | INSTR({messages.message}, 'cspdr3') |
| LENGTH | 

LENGTH(char)



 | returns the length of char | LENGTH({name}) |
| REGEXP\_INSTR | 

REGEXP\_INSTR (source\_char, pattern

\[, position

\[, occurrence

\[, return\_option

\[, match\_parameter \]

\]

\]

\]

)



 | lets you search a string for a regular expression pattern | REGEXP\_INSTR ({item.unitstype}, '\\d') |
| TO\_NUMBER() | TO\_NUMBER(expr \[, fmt \[, 'nlsparam' \] \]) | converts a formatted TEXT or NTEXT expression to a number | TO\_NUMBER({quantity}) |

## Datetime Functions {#bridgehead_N2836025}

| Function | Syntax | Short Description | Example |
| --- | --- | --- | --- |
| ADD\_MONTHS | ADD\_MONTHS(date, integer) | returns the date plus integer months | ADD\_MONTHS({today},-1) |
| LAST\_DAY | LAST\_DAY(date) | returns the date of the last day of the month that contains date | LAST\_DAY({today}) |
| MONTHS\_BETWEEN | MONTHS\_BETWEEN(date1, date2) | returns the number of months between date1 and date2 | MONTHS\_BETWEEN(SYSDATE,{createddate}) See also [Sysdate](#bridgehead_N2836722). |
| NEXT\_DAY | NEXT\_DAY(date, char) | returns the date of the first weekday named by char that is later than the date | NEXT\_DAY({today},'SATURDAY') |
| ROUND (DATE) | ROUND(date \[, fmt \]) | returns date rounded to the unit specified by the format model fmt | ROUND(TO\_DATE('12/31/2014', 'mm/dd/yyyy')-{datecreated}) |
| TO\_CHAR() | TO\_CHAR({ datetime | interval } \[, fmt \[, 'nlsparam' \] \]) | converts a datetime or interval value to a value of VARCHAR2 datatype in the format specified by the date format fmt | TO\_CHAR({date}, 'hh24') |
| TO\_DATE() | TO\_DATE(char \[, fmt \[, 'nlsparam' \] \]) | converts a formatted TEXT or NTEXT expression to a DATETIME value | TO\_DATE('31.12.2011', 'DD.MM.YYYY') |
| TRUNC (DATE) | TRUNC(date \[, fmt \]) | returns date with the time portion of the day truncated to the unit specified by the format model fmt | TRUNC({today},'YYYY') |

## NULL-Related Functions {#bridgehead_N2836356}

| Function | Syntax | Short Description | Example |
| --- | --- | --- | --- |
| COALESCE | COALESCE(expr \[, expr \]...) | returns the first non-null expr in the expression list. | COALESCE({quantitycommitted}, 0) |
| NULLIF | NULLIF(expr1, expr2) | compares expr1 and expr2. If they are equal, then the function returns null. If they are not equal, then the function returns expr1. | NULLIF({price}, 0) |
| NVL | NVL(expr1, expr2) | lets you replace null with the second parameter. | NVL({quantity},'0') |
| NVL2 | NVL2(expr1, expr2, expr3) | If expr1 is not null, then NVL2 returns expr2. If expr1 is null, then NVL2 returns expr3. | NVL2({location}, 1, 2) |

## Decode {#bridgehead_N2836578}

| Function | Syntax | Short Descriptions | Example |
| --- | --- | --- | --- |
| DECODE | 
DECODE(expr, search, result

\[, search, result \]...

\[, default \]

)



 | Compares expr to each search value one by one. If expr is equal to a search, the corresponding result is returned. If no match is found, default is returned. | DECODE({systemnotes.name}, {assigned},'T','F') |

## Sysdate {#bridgehead_N2836722}

| Function | Syntax | Short Description | Example |
| --- | --- | --- | --- |
| SYSDATE | SYSDATE | returns the current date and time set | TO\_DATE(SYSDATE, 'DD.MM.YYYY') or TO\_CHAR(SYSDATE, 'mm/dd/yyyy') See also TO\_DATE and TO\_CHAR in the [Datetime Functions](#bridgehead_N2836025). |

## Case {#bridgehead_N2839038}

| Function | Syntax | Short Description | Example |
| --- | --- | --- | --- |
| CASE | CASE { expr WHEN comparison\_expr THEN return\_expr \[ WHEN comparison\_expr THEN return\_expr \]... | WHEN condition THEN return\_expr \[ WHEN condition THEN return\_expr \]... } \[ ELSE else\_expr \] END | returns value based on different conditions | 
CASE {state}

WHEN 'NY' THEN 'New York'

WHEN 'CA' THEN 'California'

ELSE {state}

END

or

CASE

WHEN {quantityavailable} > 19 THEN 'In Stock'

WHEN {quantityavailable} > 1 THEN 'Limited Availability'

WHEN {quantityavailable} = 1 THEN 'The Last Piece'

WHEN {quantityavailable} IS NULL THEN 'Discontinued'

ELSE 'Out of Stock'

END



 |

## Analytic and Aggregate Functions {#bridgehead_N2839271}

| Function | Syntax | Short Description | Example |
| --- | --- | --- | --- |
| DENSE\_RANK | 
DENSE\_RANK(expr \[, expr \]...) WITHIN GROUP

(ORDER BY expr \[ DESC | ASC \]

\[ NULLS { FIRST | LAST } \]

\[,expr \[ DESC | ASC \]

\[ NULLS { FIRST | LAST } \]

\]...

)

or

DENSE\_RANK() OVER

(PARTITION by expr

\[,expr...\] ORDER BY expr

\[ DESC | ASC \] \[ NULLS {

FIRST | LAST } \] \[,expr \[

DESC | ASC \] \[ NULLS {

FIRST | LAST } \] \]... )



 | Computes the rank of a value with respect to other values and returns the rank as a NUMBER. Always results in consecutive rankings. | DENSE\_RANK ({amount}) WITHIN GROUP (ORDER BY {AMOUNT}) or DENSE\_RANK() OVER (PARTITION BY {name} ORDER BY {trandate} DESC) |
| KEEP() | KEEP(DENSE\_RANK { FIRST | LAST } ORDER BY expr \[ NULLS { FIRST | LAST } \]) | Qualifies an aggregate function indicating that only the FIRST or LAST values of the function are returned. | KEEP(DENSE\_RANK LAST ORDER BY {internalid}) |
| RANK | 

RANK(expr \[, expr \]...) WITHIN GROUP

(ORDER BY expr \[ DESC | ASC \]

\[ NULLS { FIRST | LAST } \]

\[, expr \[ DESC | ASC \]

\[ NULLS { FIRST | LAST } \]

\]...

)

or

RANK() OVER

(PARTITION by expr

\[,expr...\] ORDER BY expr

\[ DESC | ASC \] \[ NULLS {

FIRST | LAST } \] \[,expr \[

DESC | ASC \] \[ NULLS {

FIRST | LAST } \] \]... )



 | Computes the rank of a value in a group of values. Can result in non-consecutive rankings if values are the same. | RANK() OVER (PARTITION by {tranid} ORDER BY {line} DESC) or RANK ({amount}) WITHIN GROUP (ORDER BY {amount}) |

### Related Topics

-   [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html)
-   [Using a Custom Formula Field in a Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N660895.html)
-   [Using a Formula in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661053.html)
-   [Using a Formula in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661334.html)
-   [Using Formula Tags in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4054298146.html)
-   [Search Formula Examples and Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N662868.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
