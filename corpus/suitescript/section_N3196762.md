---
id: "section_N3196762"
type: "section"
title: "Paycheck Journal"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Paycheck Journal"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3196762.html"
anchors: ["bridgehead_N3196803", "bridgehead_N3196829"]
sha256: "ac8326d307709f0f45edf6ec2e14d00958dbc71f73784739ab3dec7c1bdcc43c"
---

The Paycheck Journal record is intended to enable global payroll solutions. You can use it along with the [Payroll Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3202912.html) record to create custom payroll solutions and to support integrations with external payroll systems.

For help working with this record in the UI, see [Paycheck Journal Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N969418.html).

The internal ID for this record is `paycheckjournal`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/paycheckjournal.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Usage Notes {#bridgehead_N3196803}

The Paycheck Journal feature must be enabled to work with the Paycheck Journal record.

## Code Samples {#bridgehead_N3196829}

The following sample creates a paycheck journal transaction.

          `// create Paycheck Journal with two earnings and one deduction sublist  function createPaycheckJournal(){      var pj = record.create ({          type: record.Type.PAYCHECK_JOURNAL,          isDynamic: true      });      pj.setValue({          fieldId: 'trandate',          value: '6/10/2012'      });        pj.setValue({          fieldId: 'employee',          value: 4                // internal ID of the employee      });        pj.setValue({          fieldId: 'account',          value: 28               // internal ID of the account      });         pj.selectNewLine({          sublistId: 'earning'      });      pj.setCurrentSublistValue({          sublistId: 'earning',          fieldId: 'payrollitem',          value: '102'      });      pj.setCurrentSublistValue({          sublistId: 'earning',          fieldId: 'amount',          value: 20.35      });          pj.commitLine({          sublistId: 'earning'      });           pj.selectNewLine({          sublistId: 'earning'      });      pj.setCurrentSublistValue({          sublistId: 'earning',          fieldId: 'payrollitem',          value: '102'      });      pj.setCurrentSublistValue({          sublistId:'earning',          fieldId: 'amount',          value: 33.35      });          pj.commitLine({          sublistId: 'earning'      });           pj.selectNewLine({          sublistId: 'deduction'      });      pj.setCurrentSublistValue({          sublistId: 'deduction',          fieldId: 'payrollitem',          value: '103'      });      pj.setCurrentSublistValue({          sublistId: 'deduction',          fieldId: 'amount',          value: 444.44      });          pj.commitLine({          sublistId: 'deduction'      });            var recordId = pj.save();  }` 
        

The following sample updates a paycheck journal transaction.

          `// update Paycheck journal by setting new amount of line 2 earning list  // and clearing the deduction list  function updatePaycheckJournal(){      var pj = record.load({          type: record.Type.PAYCHECK_JOURNAL,          isDynamic: true,          id: 305      });           pj.setSublistValue({          sublistId: 'earning',          fieldId: 'amount',          line: 2,                // 1 is the line number we intend to update          value: 444.44      });         var lineCount = pj.getLineCount({          sublistId: 'deduction'      });      for (var lineNo = 1; lineNo <= lineCount; lineNo++) {                pj.removeLine({              sublistId: 'deduction',              line: lineNo          });      }     var recId = pj.save();  }` 
        

### Related Topics

-   [Paycheck Journal Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N969418.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
