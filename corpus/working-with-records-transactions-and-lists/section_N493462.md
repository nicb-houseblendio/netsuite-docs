---
id: "section_N493462"
type: "section"
title: "Creating a Static Group"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Working with Groups > Creating a Static Group"
parent: "section_N492945"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N493462.html"
anchors: []
sha256: "9f9638d582a756e697db07fd79051119caf4a22c4c8af5fad76970a6c8fe599a"
---

The membership of a static group remains constant. You can create static groups by selecting members from lists and with a search. Support and sales groups must be static groups.

You can also use CSV Import to create and update static groups. For more information, see [Group Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159282407440.html).

You can add or remove members from a static group at any time.

Note:

You can't create a static group with more than 10,000 members. For groups larger than 10,000, you must create a dynamic group.

#### To create a Static Group:

1.  Go to _Lists > Relationships > Groups_ > New.
    
2.  On the **Create Group** page, choose **Static**.
    
3.  Choose the kind of members you would like this group to contain.
    
4.  Click **Continue**.
    
5.  Enter a name for this group.
    
6.  If applicable, complete the following:
    
    -   If the owner of this group is someone else, select that person in the **Owner** field.
        
    -   If this group shares an email alias, enter the email address in the **Email** field.
        
    -   Enter other information about this group in the **Comments** field.
        
    -   Check the **Private** box if you want to restrict viewing (and also editing) of this group to its members.
        
    -   If you want to restrict access to this group to members of another group, select the group in the **Restrict To** field.
        
        Note:
        
        Restricted groups can't be marked private. Restricted groups can only be used by members of the group you select in the **Restrict To** field.
        
    -   Check the **Restrict Group Editing to Owner** box if you want to restrict editing permissions to the group owner as specified in the **Owner** field.
        
        You should enable the **Restrict Group Editing to Owner** preference whenever you're setting up a group to control access to sensitive information. For example, when restricting access to certain File Cabinet folders.
        
        If you want to grant other members of the group editing permissions, either make the group private or restrict it to another group by enabling the relevant setting on the group records page. Don't place sensitive material in a File Cabinet folder that's accessible from a public group.
        
        Also ensure that the role used to access the group has an appropriate CRM Groups access level assigned to it on the relevant manage roles page. (Go to _Setup > Users > Role > Manage Roles_.)
        
        If you disable **Restrict Group Editing to Owner** and choose to make your group public, any user with access to a role with edit-level access to CRM Groups, can access and edit your group's content. This includes access to File Cabinet folders as well as adding and deleting members.
        
        For more information about assigning role-based permissions, see [Reviewing Permissions Assigned to Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326209.html).
        
7.  If you're creating an employee group, the following fields are available:
    
    -   **Support Group** - Check this box to mark this group a support group.
        
        On case records, support groups are listed in the **Assigned To** field. When you assign a case territory, support groups are listed in the **Support Rep.** field.
        
    -   **Product Team** - Check this box to mark this group as a product team.
        
        Product team groups can be selected in the **Product Team** field on issues. Product teams designate who's responsible for resolving an issue. Members of this team are emailed when an issue is first entered so that everyone is aware of the problem.
        
    -   **Functional Team** - Check this box to mark this group as a functional team.
        
        Functional teams can be emailed copies of the issue from the **Communication** subtab on issue records. You may want to check this box for all product team groups and then create additional function team groups for other teams you want to email.
        
    -   **Issue Role** - Select a role that corresponds to the role of this group's members, and this group can be assigned to issues.
        
8.  On the **Members** subtab, do one or more of the following:
    
    -   To add individual members, enter part of a member's name in the **Name** column, and press Tab. Select a member, and click **Add**. Repeat these steps for each member.
        
    -   Click **Add Multiple**, and hold the Ctrl key to select more than one member from the list.
        
    -   Click **Add With Search** to enter search criteria for the members you want to add.
        
        You can use more than one of these methods to add members to the same group. For example, you can select a few members individually and then add all the members that meet search criteria.
        

Depending on the kind of group you're creating, you can use joined searches to generate your results. For example, if you're creating a customer group, you can use a transaction search to give you the desired results. If you're creating a contact group, you can search for vendors that meet the criteria.

Note:

To access a Group's calendar, use the dropdown menu below the date selector on the calendar portlet.

To add a member to this group, open the group record. On the **Members** subtab, use one of the methods in step 8 to add a member.

To remove a member from this group, open the group record. On the **Members** subtab, click **Remove** on the row of the member you want to remove.

### Related Topics

-   [Working with Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N492945.html)
-   [Creating a Dynamic Group](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N493194.html)
-   [Creating a Contact Group](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N493826.html)
-   [Adding and Removing Members of Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1502138792.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
