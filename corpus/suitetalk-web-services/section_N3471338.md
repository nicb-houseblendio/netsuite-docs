---
id: "section_N3471338"
type: "section"
title: "Platform Enumerations"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Types > Platform Enumerations"
parent: "chapter_N3452524"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html"
anchors: []
sha256: "873721265aa47c213f3caabecb074894a52f6c7031a6198acf9ff1d168c020a4"
---

The following search types are used throughout SOAP web services to populate system defined lists. The tables below outline the available values that should be used to populate these fields in your SOAP web services requests. These enumerations are defined in the [platformCoreTyp XSD](https://webservices.netsuite.com/xsd/platform/v2025_2_0/coreTypes.xsd).

| Search Types (Table 1) |  |
| --- | --- |
| Enumerations | 
SearchString

FieldOperator



 | SearchLongFieldOperator | SearchDoubleFieldOperator | 

SearchPeriod

Field



 | 

SearchTime

FieldOperator



 |
| --- | --- | --- | --- | --- | --- |
| is | X |  |  |  |  |
| isNot | X |  |  |  |  |
| startsWith | X |  |  |  |  |
| doesNotStartWith | X |  |  |  |  |
| contains | X |  |  |  |  |
| doesNotContain | X |  |  |  |  |
| equalTo |  | X | X | X |  |
| lessThan |  | X | X |  |  |
| greaterThan |  | X | X |  |  |
| lessThanOrEqualTo |  | X | X |  |  |
| greaterThanOrEqualTo |  | X | X |  |  |
| notEqualTo |  | X | X |  |  |
| notLessThan |  | X | X |  |  |
| notGreaterThan |  | X | X |  |  |
| notLessThanOrEqualTo |  | X | X |  |  |
| notGreaterThanOrEqualTo |  | X | X |  |  |
| between |  | X | X |  | X |
| notBetween |  | X | X |  |  |
| empty |  | X | X |  |  |
| notEmpty |  | X | X |  |  |

| Search Types (Table 2) |
| --- |
| Enumerations | 
SearchDate

FieldOperator



 | 

SearchEnum

MultiSelect

FieldOperator



 | 

SearchMulti

SelectField

Operator



 | SearchDate |
| --- | --- | --- | --- | --- |
| anyOf |  | X | X |  |
| noneOf |  | X | X |  |
| on | X |  |  |  |
| before | X |  |  |  |
| after | X |  |  |  |
| onOrBefore | X |  |  |  |
| onOrAfter | X |  |  |  |
| within | X |  |  |  |
| empty | X |  |  |  |
| notOn | X |  |  |  |
| notBefore | X |  |  |  |
| notAfter | X |  |  |  |
| notOnOrBefore | X |  |  |  |
| notOnOrAfter | X |  |  |  |
| notWithin | X |  |  |  |
| notEmpty | X |  |  |  |
| fiscalHalfBeforeLast |  |  |  | X |
| fiscalHalfBeforeLastToDate |  |  |  | X |
| fiscalQuarterBeforeLast |  |  |  | X |
| fiscalQuarterBeforeLastToDate |  |  |  | X |
| fiscalYearBeforeLast |  |  |  | X |
| fiscalYearBeforeLastToDate |  |  |  | X |
| fiveDaysAgo |  |  |  | X |
| fiveDaysFromNow |  |  |  | X |
| fourDaysAgo |  |  |  | X |
| fourDaysFromNow |  |  |  | X |
| fourWeeksStartingThisWeek |  |  |  | X |
| lastBusinessWeek |  |  |  | X |
| lastFiscalHalf |  |  |  | X |
| lastFiscalHalfOneFiscalYearAgo |  |  |  | X |
| lastFiscalHalfToDate |  |  |  | X |
| lastFiscalQuarter |  |  |  | X |
| lastFiscalQuarterOneFiscalYearAgo |  |  |  | X |
| lastFiscalQuarterToDate |  |  |  | X |
| lastFiscalQuarterTwoFiscalYearsAgo |  |  |  | X |
| lastFiscalYear |  |  |  | X |
| lastFiscalYearToDate |  |  |  | X |
| lastMonth |  |  |  | X |
| lastMonthOneFiscalQuarterAgo |  |  |  | X |
| lastMonthOneFiscalYearAgo |  |  |  | X |
| lastMonthToDate |  |  |  | X |
| lastMonthTwoFiscalQuartersAgo |  |  |  | X |
| lastMonthTwoFiscalYearsAgo |  |  |  | X |
| lastRollingHalf |  |  |  | X |
| lastRollingQuarter |  |  |  | X |
| lastRollingYear |  |  |  | X |
| lastWeek |  |  |  | X |
| lastWeekToDate |  |  |  | X |
| monthAfterNext |  |  |  | X |
| monthAfterNextToDate |  |  |  | X |
| monthBeforeLast |  |  |  | X |
| monthBeforeLastToDate |  |  |  | X |
| nextBusinessWeek |  |  |  | X |
| nextFiscalHalf |  |  |  | X |
| nextFiscalQuarter |  |  |  | X |
| nextFiscalYear |  |  |  | X |
| nextFourWeeks |  |  |  | X |
| nextMonth |  |  |  | X |
| nextOneHalf |  |  |  | X |
| nextOneMonth |  |  |  | X |
| nextOneQuarter |  |  |  | X |
| nextOneWeek |  |  |  | X |
| nextOneYear |  |  |  | X |
| nextWeek |  |  |  | X |
| ninetyDaysAgo |  |  |  | X |
| ninetyDaysFromNow |  |  |  | X |
| oneYearBeforeLast |  |  |  | X |
| previousFiscalQuartersLastFiscalYear |  |  |  | X |
| previousFiscalQuartersThisFiscalYear |  |  |  | X |
| previousMonthsLastFiscalHalf |  |  |  | X |
| previousMonthsLastFiscalQuarter |  |  |  | X |
| previousMonthsLastFiscalYear |  |  |  | X |
| previousMonthsSameFiscalHalfLastFiscalYear |  |  |  | X |
| previousMonthsSameFiscalQuarterLastFiscalYear |  |  |  | X |
| previousMonthsThisFiscalHalf |  |  |  | X |
| previousMonthsThisFiscalQuarter |  |  |  | X |
| previousMonthsThisFiscalYear |  |  |  | X |
| previousOneDay |  |  |  | X |
| previousOneHalf |  |  |  | X |
| previousOneMonth |  |  |  | X |
| previousOneQuarter |  |  |  | X |
| previousOneWeek |  |  |  | X |
| previousOneYear |  |  |  | X |
| previousRollingHalf |  |  |  | X |
| previousRollingQuarter |  |  |  | X |
| previousRollingYear |  |  |  | X |
| sameDayFiscalQuarterBeforeLast |  |  |  | X |
| sameDayFiscalYearBeforeLast |  |  |  | X |
| sameDayLastFiscalQuarter |  |  |  | X |
| sameDayLastFiscalYear |  |  |  | X |
| sameDayLastMonth |  |  |  | X |
| sameDayLastWeek |  |  |  | X |
| sameDayMonthBeforeLast |  |  |  | X |
| sameDayWeekBeforeLast |  |  |  | X |
| sameFiscalHalfLastFiscalYear |  |  |  | X |
| sameFiscalHalfLastFiscalYearToDate |  |  |  | X |
| sameFiscalQuarterFiscalYearBeforeLast |  |  |  | X |
| sameFiscalQuarterLastFiscalYear |  |  |  | X |
| sameFiscalQuarterLastFiscalYearToDate |  |  |  | X |
| sameMonthFiscalQuarterBeforeLast |  |  |  | X |
| sameMonthFiscalYearBeforeLast |  |  |  | X |
| sameMonthLastFiscalQuarter |  |  |  | X |
| sameMonthLastFiscalQuarterToDate |  |  |  | X |
| sameMonthLastFiscalYear |  |  |  | X |
| sameMonthLastFiscalYearToDate |  |  |  | X |
| sameWeekFiscalYearBeforeLast |  |  |  | X |
| sameWeekLastFiscalYear |  |  |  | X |
| sixtyDaysAgo |  |  |  | X |
| sixtyDaysFromNow |  |  |  | X |
| startOfFiscalHalfBeforeLast |  |  |  | X |
| startOfFiscalQuarterBeforeLast |  |  |  | X |
| startOfFiscalYearBeforeLast |  |  |  | X |
| startOfLastBusinessWeek |  |  |  | X |
| startOfLastFiscalHalf |  |  |  | X |
| startOfLastFiscalHalfOneFiscalYearAgo |  |  |  | X |
| startOfLastFiscalQuarter |  |  |  | X |
| startOfLastFiscalQuarterOneFiscalYearAgo |  |  |  | X |
| startOfLastFiscalYear |  |  |  | X |
| startOfLastMonth |  |  |  | X |
| startOfLastMonthOneFiscalQuarterAgo |  |  |  | X |
| startOfLastMonthOneFiscalYearAgo |  |  |  | X |
| startOfLastRollingHalf |  |  |  | X |
| startOfLastRollingQuarter |  |  |  | X |
| startOfLastRollingYear |  |  |  | X |
| startOfLastWeek |  |  |  | X |
| startOfMonthBeforeLast |  |  |  | X |
| startOfNextBusinessWeek |  |  |  | X |
| startOfNextFiscalHalf |  |  |  | X |
| startOfNextFiscalQuarter |  |  |  | X |
| startOfNextFiscalYear |  |  |  | X |
| startOfNextMonth |  |  |  | X |
| startOfNextWeek |  |  |  | X |
| startOfPreviousRollingHalf |  |  |  | X |
| startOfPreviousRollingQuarter |  |  |  | X |
| startOfPreviousRollingYear |  |  |  | X |
| startOfSameFiscalHalfLastFiscalYear |  |  |  | X |
| startOfSameFiscalQuarterLastFiscalYear |  |  |  | X |
| startOfSameMonthLastFiscalQuarter |  |  |  | X |
| startOfSameMonthLastFiscalYear |  |  |  | X |
| startOfThisBusinessWeek |  |  |  | X |
| startOfThisFiscalHalf |  |  |  | X |
| startOfThisFiscalQuarter |  |  |  | X |
| startOfThisFiscalYear |  |  |  | X |
| startOfThisMonth |  |  |  | X |
| startOfThisWeek |  |  |  | X |
| startOfThisYear |  |  |  | X |
| startOfWeekBeforeLast |  |  |  | X |
| tenDaysAgo |  |  |  | X |
| tenDaysFromNow |  |  |  | X |
| thirtyDaysAgo |  |  |  | X |
| thirtyDaysFromNow |  |  |  | X |
| thisBusinessWeek |  |  |  | X |
| thisFiscalHalf |  |  |  | X |
| thisFiscalHalfToDate |  |  |  | X |
| thisFiscalQuarter |  |  |  | X |
| thisFiscalQuarterToDate |  |  |  | X |
| thisFiscalYear |  |  |  | X |
| thisFiscalYearToDate |  |  |  | X |
| thisMonth |  |  |  | X |
| thisMonthToDate |  |  |  | X |
| thisRollingHalf |  |  |  | X |
| thisRollingQuarter |  |  |  | X |
| thisRollingYear |  |  |  | X |
| thisWeek |  |  |  | X |
| thisWeekToDate |  |  |  | X |
| thisYear |  |  |  | X |
| threeDaysAgo |  |  |  | X |
| threeDaysFromNow |  |  |  | X |
| threeFiscalQuartersAgo |  |  |  | X |
| threeFiscalQuartersAgoToDate |  |  |  | X |
| threeFiscalYearsAgo |  |  |  | X |
| threeFiscalYearsAgoToDate |  |  |  | X |
| threeMonthsAgo |  |  |  | X |
| threeMonthsAgoToDate |  |  |  | X |
| today |  |  |  | X |
| tomorrow |  |  |  | X |
| twoDaysAgo |  |  |  | X |
| twoDaysFromNow |  |  |  | X |
| weekAfterNext |  |  |  | X |
| weekAfterNextToDate |  |  |  | X |
| weekBeforeLast |  |  |  | X |
| weekBeforeLastToDate |  |  |  | X |
| yesterday |  |  |  | X |

Important:

The onOrAfter, onOrBefore, notOnOrAfter and notOnOrBefore operators only consider the date you specify in your request, and ignore the time you specify. If you need to specify not only the date but also the time in your search, use the after or before operators. Note, however, when you use these operators, the exact time specified in your request is not part of the result set.

### Related Topics

-   [Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3452524.html)
-   [Built-in Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452691.html)
-   [Complex Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452954.html)
-   [Custom Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3458179.html)
-   [Search Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3460474.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
