---
id: "chapter_N3184398"
type: "chapter"
title: "Entities"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Entities"
parent: "chapter_N3170023"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3184398.html"
anchors: ["bridgehead_1505832354", "bridgehead_1505833511"]
sha256: "e4dd1b5bbc78425578b9e8b4b100c8b32fbdd5b7d6fcffd948f60db89eaa74d2"
---

## Entity Record Restrictions for Scripting on Administrator Role {#bridgehead_1505832354}

This section describes entity record restrictions for scripting on the Administrator and Full permissions roles. Note that these restrictions apply to all versions of SuiteScript and all NetSuite environments (see [Understanding NetSuite Account Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4413974567.html)).

You cannot perform these actions with SuiteScript:

-   Create an entity record where any role is set to Administrator or Full permissions
    
-   Delete an entity record where any role is set to Administrator or Full permissions
    
-   Edit an entity record so that the entity gains an Administrator role
    
-   Edit an entity record so that the entity loses an Administrator role
    
-   Edit the password or email field value on an entity record where any role is set to Administrator or Full permissions
    

These restrictions contribute to improved security. Scripts that break them throw an error message: `Script Security Violation: Unauthorized attempt to <operation> entity with <role> role by SuiteScript!`

## Entity Record Types {#bridgehead_1505833511}

The following entity records are scriptable in SuiteScript:

-   [As Charged Project Revenue Rule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_80125913437.html)
    
-   [Bonus](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157373984745.html)
    
-   [Bonus Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157374008038.html)
    
-   [Competitor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3184614.html)
    
-   [Contact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3184656.html)
    
-   [Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3184698.html)
    
-   [Customer Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4858833375.html)
    
-   [Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3185342.html)
    
-   [Employee Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156278523556.html)
    
-   [Employee Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156278524821.html)
    
-   [Entity](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3185716.html)
    
-   [Entity Group](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0302025324.html)
    
-   [Generic Resource](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4230622268.html)
    
-   [Job](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497637078.html)
    
-   [Job Requisition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497637105.html)
    
-   [Lead](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3186192.html)
    
-   [Other Name](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3187056.html)
    
-   [Partner](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3187098.html)
    
-   [Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3185758.html)
    
-   [Project Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4858840833.html)
    
-   [Project Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4206752382.html)
    
-   [Project Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4858841256.html)
    
-   [Prospect](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3187339.html)
    
-   [Time-Off Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497626640.html)
    
    -   [Time-Off Change](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497626640.html#bridgehead_4583287478)
        
    -   [Time-Off Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497626640.html#bridgehead_4583284469)
        
    -   [Time-Off Request](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497626640.html#bridgehead_4583285968)
        
    -   [Time-Off Rule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497626640.html#bridgehead_4583287919)
        
    -   [Time-Off Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497626640.html#bridgehead_4583286901)
        
-   [Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3187808.html)
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
