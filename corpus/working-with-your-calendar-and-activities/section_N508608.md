---
id: "section_N508608"
type: "section"
title: "Creating CRM Task Records"
branch: "working-with-your-calendar-and-activities"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Your Calendar and Activities > Working with CRM Tasks > Creating CRM Task Records"
parent: "section_N506499"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N508608.html"
anchors: ["procedure_N508666"]
sha256: "4a840c39cb6607f37a63ee34cd7ee9b6ebe5145878a65389a77818a616d2540f"
---

Create a new CRM task record to track work items that need to be completed. Administrators can use the Import Assistant to import CRM tasks from another system into NetSuite. For more information, see [Tasks Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N360296.html).

To track tasks associated with projects, use Project Task records. For more information, see [Project Task Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html#bridgehead_N1192945).

To set a preference for CRM Tasks to display on your calendar, go to _Activities > Setup > Calendar Preference_ > Preferences subtab. Check the Display Non-blocking Tasks in Calendar box.

#### To create a CRM task: {#procedure_N508666}

1.  Open a new task record by doing one of the following:
    
    -   Go to Activities > Scheduling > Tasks and click **New**.
        
    -   Click **Task** in the Create New menu.
        
2.  In the Primary Information field group:
    
    -   Select the form you want to use in the **Custom Form** field. This field appears only if multiple task forms are available.
        
    -   Enter a **Title** for the task. The title should describe the task.
        
    -   In the **Assigned To** field, select the employee who is assigned to the task.
        
        Your name appears in this field by default.
        
        Note:
        
        In NetSuite OneWorld accounts, employees from all subsidiaries show in this field.
        
    -   Check the **Notify Assignee by Email** box to send an email notification to the assigned person. This email informs the person that a task has been created or edited and assigned to them. If this person's record doesn't have an email address, no message is sent.
        
    -   Select the appropriate level of priority for this task.
        
    -   Use the **Insert Before** field to change the order of tasks. Select a task from the list that the new task should be placed above.
        
    -   Select a **Status** for this task. Only someone with permission to edit the task record can change the status.
        
    -   (Optional) Check the **Private Task** box if you want only you or the person in the **Assigned To** field to see this task. If you also use Time Tracking for CRM, only the person assigned to a private task can track time against the task.
        
3.  In the Date and Time field group:
    
    -   Set the **Start Date** for this task.
        
    -   In the **Due Date** field, enter the date when this task should be completed.
        
    -   After the task is finished, fill in the **Date Completed** field.
        
        Note:
        
        You can edit the value in the Date Completed field even after you set the Status to Completed.
        
    -   (Optional) Check the **Reserve Time** box to turn the task into a scheduled task which can be displayed on the calendar. When you check this box, the **Start Time** and **End Time** fields become required fields.
        
        -   Select the **Start Time** and **End Time**.
            
            Note:
            
            Use the **Availability** subtab to view when the person assigned to the task is available.
            
        -   In the **Reminder Type** field, select a type of reminder for scheduled tasks that appear on the calendar:
            
            **None** - No reminder is triggered.
            
            **Email** - An email reminder is sent to the email address on the employee record for the person selected in the Assigned To field.
            
            **Popup** - A popup reminder opens when the person assigned to this task is logged in to NetSuite.
            
        -   In the **Reminder** field, select a time before the task begins when you want to see the reminder.
            
            Note:
            
            You must select both a **Reminder Type** and a **Reminder** time to trigger the reminder. The person assigned to this task can edit the task record to change the reminder settings.
            
4.  Review and edit other subtabs as necessary.
    
    **Message** subtab:
    
    In the **Message** field, enter notes or a description about this task. These comments appear in the email message sent to the person this task is assigned to.
    
    Optionally, you can get writing help for the field using our generative AI service, NetSuite Text Enhance. Click the Enhance Text button to use the available options. For more information about using this capability, see [Text Enhance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2171112518.html).
    
    **Related Records** subtab:
    
    -   Select a **Company** if this task is related to a customer, vendor, partner, or other name.
        
    -   The **Contact** field lists the contacts for the company you've selected. Select the contact associated with the task.
        
    -   If this task is related to a support case, select the case number in the **Support Case** field.
        
    -   If this task is related to a transaction, select the transaction number in the **Transaction** field.
        
    -   Select and add multiple companies and contacts associated with this task.
        
        For example, you can add the contact who requested the task or requires reporting on this task in the **Companies and Contacts** list.
        
    
    **Availability** subtab - Displays the availability of the user assigned to the task.
    
    **Communication** subtab:
    
    -   Click the **Files** subtab to attach a file to this event. For more information about attaching files, see [Attaching Files to Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N490137.html).
        
    -   Click the **User Notes** subtab to add any notes about this event.
        
    
    **Time Tracking** subtab:
    
    If you've enabled either the Time Tracking for CRM or Project Management feature, you can track time for this task. For more information, see [Tracking Time on CRM Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N509136.html).
    
5.  After you've filled in information about these subtabs, click **Save**.
    

You can change or update existing tasks by clicking Edit next to a task from the tasks list.

As you work on your tasks or complete them, update the status of the tasks. If the tasks aren't marked private, others can see your progress and know what you're working on. This facilitates communication between departments within your company.

### Additional Information

-   [Personal Preferences for Activities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N482375.html)

### Related Topics

-   [Working with CRM Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N506499.html)
-   [Tracking Time on CRM Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N509136.html)
-   [Tasks and Project Tasks Portlets on Your Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N509646.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
