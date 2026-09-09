---
id: "section_N493194"
type: "section"
title: "Creating a Dynamic Group"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Working with Groups > Creating a Dynamic Group"
parent: "section_N492945"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N493194.html"
anchors: ["procedure_N493213"]
sha256: "c66c1ce741437966f2d909987213e26ce7b6c96a242ecde574c0043e17d1ea11"
---

Dynamic group membership changes to include anyone who meets the criteria defined in a saved search.

For example, you can set search criteria to create a group of all employee sales reps. When a new sales rep is hired, the rep automatically becomes a member of this dynamic group. When a sales rep takes a position in another department, that rep is removed from the group automatically. Whenever you use the Mail Merge feature to send bulk email to this dynamic group, NetSuite uses the search criteria to determine the current group members.

You can create a dynamic group from an existing saved search or you can create a new saved search when you create the group.

#### To create a dynamic group: {#procedure_N493213}

1.  Go to _Lists > Relationships > Groups_ > New.
    
2.  On the **Create Group** page, choose **Dynamic**.
    
3.  Choose the kind of members you would like this group to contain.
    
4.  Click **Continue**.
    
5.  Enter a name for this group.
    
6.  Select an existing saved search in the **Saved Search** list.
    
    -   Only saved searches that include the kind of members you selected in step 3 appear in the list.
        
    -   For more information about saved searches, see [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html).
        
        Depending on the kind of group you're creating, you can use joined searches to generate your results. For example, if you're creating a customer group, you can use a transaction search to give you the desired results. If you're creating a contact group, you can search for vendors that meet the criteria.
        
        After you select or create a saved search, the members of the group are shown on the **Members** subtab.
        
7.  If the owner of this group is someone else, select that person in the **Owner** field.
    
    Note:
    
    Owners for dynamic groups and saved searches are configured separately. Only the owner of the saved search can save changes when editing a saved search.
    
8.  (Optional) If this group shares an email alias, enter the email address in the **Email** field.
    
9.  (Optional) Enter other information about this group in the **Comments** field.
    
10.  (Optional) Check the **Private** box if you want to restrict viewing (and also editing) of this group to its members.
     
11.  (Optional) If you want to restrict access to this group to members of another group, select the group in the **Restrict To** field.
     
     Note:
     
     Restricted groups can't be marked private. Restricted groups can only be used by members of the group you select in the **Restrict To** field.
     
12.  (Optional) Clear the **Restrict Group Editing to Owner** box if you want to allow other group members to edit this group. By default, this box is checked.
     
     You should check the **Restrict Group Editing to Owner** box when you set up a group that controls access to sensitive information such as access to particular File Cabinet folders.
     
     If you intend to grant other members of the group editing permissions, You should either make the group private or restrict it to another group by enabling the relevant setting on the group records page. Don't store sensitive material in a File Cabinet folder that is accessible from a public group.
     
     You should also ensure that the role used to access the group has an appropriate CRM Groups access level assigned to it on the relevant manage roles page. Go to _Setup > Users > Role > Manage Roles_.
     
     If you clear the **Restrict Group Editing to Owner** box and choose to make your group public, any user with access to a role with edit-level access to CRM Groups can access and edit your group's content. This includes access to File Cabinet folders as well as adding and deleting members.
     
     For more information about assigning role-based permissions, see [Reviewing Permissions Assigned to Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326209.html).
     
13.  Click **Save**.
     

Now, every time a record of this type is created, it's added to this group if it matches the criteria in the saved search.

### Related Topics

-   [Working with Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N492945.html)
-   [Creating a Static Group](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N493462.html)
-   [Creating a Contact Group](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N493826.html)
-   [Adding and Removing Members of Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1502138792.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
