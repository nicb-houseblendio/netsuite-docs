---
id: "section_N3691883"
type: "section"
title: "Time Bill (Track Time)"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions-related Records > Time Bill (Track Time)"
parent: "article_160526452785"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3691883.html"
anchors: ["bridgehead_N3691928", "bridgehead_N3692142", "bridgehead_N3692180", "bridgehead_4788102974", "bridgehead_4788102309", "bridgehead_N3692192", "bridgehead_N28494231"]
sha256: "73661a1f249e20c8d35f6040cb7a6458cc9e9e66ffaa4a5181ccc2b190b60a19"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Time Bill (Track Time)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164439865832.html).

A time transaction, also known as TimeBill, records the hours worked by an employee. This transaction can be used to record billable hours and invoice customers. This transaction is available when the Time Tracking feature is enabled.

For details about this type of transaction, [Managing Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901953.html).

The TimeBill record is defined in the [tranEmp (employees)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/employees.xsd) XSD.

Important:

The TimeBill record is labelled as the Track Time record in the UI.

## Supported Operations {#bridgehead_N3691928}

The following operations can be used with TimeBill records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3692142}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [time bill](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/timebill.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3692180}

## Weekly Timesheets {#bridgehead_4788102974}

The Weekly Timesheets feature works in conjunction with the Time Tracking feature. For more information about the Weekly Timesheets feature, see [Weekly Timesheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4671374137.html).

The TimeBill record used for the Time Tracking feature is supported when the Weekly Timesheets feature is enabled. Each TimeBill instance is a standalone record that belongs to only one TimeSheet instance. The TimeBill record's read-only RecordRef field, timeSheet references the TimeSheet to which each TimeBill belongs.

When the Weekly Timesheets feature is enabled, each TimeSheet references its related TimeBills in the timeitem sublist. A single TimeSheet can reference multiple TimeBills.

TimeBills are not available currently through the TimeSheet record in SOAP web services. To get all TimeBills for a TimeSheet, use TimeBill search.

The timeSheet field is available to TimeBill searches. You can also use joins for the TimeSheet and TimeBill searches.

## Price Field {#bridgehead_4788102309}

As of the 2011.2 endpoint, if you create a time bill record with a Price field set to -1, the value of the field is blank, rather than Custom.

## Adding a Time Bill {#bridgehead_N3692192}

The following code shows how to add a time bill.

## C# {#bridgehead_N28494231}

          `private void addTimeBill() {    Console.WriteLine("\nEnter Employee name: ");      // Look for the employee    EmployeeSearch empSearch = new EmployeeSearch();    SearchStringField employeeEntityID = new SearchStringField();    employeeEntityID.@operator = SearchStringFieldOperator.@is;    employeeEntityID.operatorSpecified = true;    employeeEntityID.searchValue = Console.ReadLine();      EmployeeSearchBasic empBasic = new EmployeeSearchBasic();    empBasic.entityId = employeeEntityID;      empSearch.basic = empBasic;      // Run the search     SearchResult result = _service.search(empSearch);      if (result.status.isSuccess)    {       Console.WriteLine("\nEmployees found: " + result.recordList.Length);         if (result.recordList != null && result.recordList.Length == 1)       {          Employee emp = (Employee)result.recordList[0];            Console.WriteLine("\nEmployeeID: " + emp.internalId);            // Instantiate new blank time bill record          TimeBill timeBill = new TimeBill();            // Instantiate a record object          timeBill.employee = new RecordRef();           timeBill.employee.type = RecordType.employee;          timeBill.employee.internalId = emp.internalId;            // Set the date of the time bill to today          timeBill.tranDate = DateTime.Today;          Console.WriteLine("\nToday: {0}", timeBill.tranDate);            // Get the amount of hours to add          timeBill.hours = new Duration();          Console.WriteLine("\nEnter hours: ");            // Convert the string to a double          timeBill.hours.timeSpan = Double.Parse(Console.ReadLine());            // Add the record          WriteResponse response = _service.add(timeBill);            // Display the result of the operation          if(response.status.isSuccess)          {             Console.WriteLine("Record added");          }          else          {             Console.WriteLine("Record was not added");          }       }       else       {          Console.WriteLine("\nSorry - No such Employee");       }    } }` 
        

### Related Topics

-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Usage Notes for Transaction Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3658677.html)
-   [Transaction Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659492.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
