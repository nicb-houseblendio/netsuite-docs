---
id: "section_N2344727"
type: "section"
title: "Creating Manufacturing Work Centers or Groups"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Routing > Setting Up Manufacturing Routing > Creating Manufacturing Work Centers or Groups"
parent: "section_N2341463"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2344727.html"
anchors: ["procedure_N2344778"]
sha256: "39a18ac1a8380fcc543e713786c36a73e2b8bb726e2e17f58ddf6faa1687f6ca"
---

A work center is a group of people that perform a specific step in the manufacturing process. After you define a work center group, that work center can be assigned to cover specific steps in the manufacturing process. For example, your assembly process might require the following groups: manufacturing, quality assurance, and packing machine.

You create work centers by creating a static group, and then identifying it as a manufacturing work center.

#### To create a manufacturing work center: {#procedure_N2344778}

1.  Go to Go to Lists > Relationships > Groups > New.
    
2.  Select **Static** as the kind of group.
    
3.  Select **Employee** as the kind of members.
    
4.  Click **Continue**.
    
5.  On Create Static Employee Group page, enter a name for this group.
    
    For example, enter **Packing Machine Group**. This name shows in work center lists on records and forms.
    
6.  Select the owner of this group.
    
    Note:
    
    You are selected by default. Only the owner of a group can add or remove members or delete the group.
    
7.  Check the **Manufacturing Work Center** box. This enables this group to be used as a work center with routing records.
    
8.  Click the **Manufacturing Work Center Settings** subtab.
    
9.  Select one or more locations to associate with this work center.
    
    If you use NetSuite OneWorld, you can select multiple locations within a subsidiary.
    
10.  Enter the number of machine resources for this work center.
     
     If this machine is used in multiple work centers, enter a decimal amount. For example, if this machine is used by another work center for half the day, enter 0.5.
     
11.  Enter number of labor resources for this work center.
     
     If labor is used by multiple work centers, enter a decimal amount. For example, if a welder spends only two hours in this work center in a day, enter 0.25.
     
12.  Complete any additional fields necessary for this group record.
     
13.  Click **Save**.
     

NetSuite uses the associated work calendar to schedule the operation tasks associated with each work center.

For more information about creating a static group record, read [Creating a Static Group](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N493462.html).

### Related Topics

-   [Setting Up Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2341463.html)
-   [Enabling the Manufacturing Routing Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2341773.html)
-   [Setting Routing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3950900044.html)
-   [Defining Cost Categories for Manufacturing Routing and Work Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2342063.html)
-   [Defining a Manufacturing Charge Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2343650.html)
-   [Creating Manufacturing Cost Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2344013.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
