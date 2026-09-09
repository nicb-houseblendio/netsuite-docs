---
id: "section_N501988"
type: "section"
title: "Creating a New Event Record"
branch: "working-with-your-calendar-and-activities"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Your Calendar and Activities > Working with Events > Scheduling Events > Creating a New Event Record"
parent: "section_N501467"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N501988.html"
anchors: ["procedure_N502033"]
sha256: "e7922f8aa3c480d2e9bfd22c5e28e4edee4a2e4a9718eb16b7b4a39d050793b5"
---

Use an event record to send an email invitation, attach a document for discussion, and to reserve a resource such as a conference room.

When you create an event, you're the owner and automatically designated as the organizer. Only you can create events on your calendar. The event's organizer, owner, or any role who has edit- or full-level permissions to events on your calendar can make changes to the event records including assigning or changing organizers.

Note:

Administrators can view, edit, or delete any task, event or call, even if it's not assigned to them and regardless of the event's access settings.

#### To create a new event record: {#procedure_N502033}

1.  Go to _Activities > Scheduling > Events > New_.
    
2.  Under Primary Information:
    
    1.  You can select a Custom Form (optional).
        
    2.  In the **Title** field, enter the subject or title for this event.
        
    3.  Fill in the **Location** field, and select the date of this event.
        
    4.  Select whether the status of the event is **Confirmed, Tentative** or **Canceled**.
        
    5.  In the **Event Access** field, select how you want this event to appear on your calendar.
        
        -   **Public** - Everyone with access to the calendar can see this event and its details.
            
        -   **Private** - This event appears only to you and to invitees with access to the calendar. For more information, see [Event Scheduling Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N502623.html).
            
        -   **Show as Busy** - This event appears as a busy time slot to everyone with access to the calendar. No other information about this event is shown.
            
    6.  In the **Organizer** field, select the person who's organizing this event. The event organizer is automatically set as an accepted attendee for this event.
        
        If you change the organizer, the new organizer isn't automatically added to the attendee list.
        
3.  Under Date and Time:
    
    1.  Select a date for the event.
        
    2.  Check the **All Day** box, if the event lasts all day.
        
        When you check this box, the start and end times fill in automatically based on your calendar preferences.
        
        Note:
        
        If you need to create an event that spans multiple days, create an all day event for the first day, and on the Recurrence subtab, choose Daily and set the last day of the event in the End By field.
        
    3.  Check the **Reserve Time** box if you want to reserve time on your calendar for this event.
        
        Events that don't reserve time appear first on your calendar for that day-for example, birthdays or anniversaries.
        
    4.  Select the start and end times for this event. If the selected time slot conflicts with any existing events, you'll get a popup warning.
        
    5.  In the **Reminder Type** field select the type of reminder you want to get.
        
    6.  In the **Reminder** field, select a time before the event when you want to be reminded. For more information, see [Setting Up Event Reminders when Creating or Editing Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N505393.html).
        
4.  On the **Message** subtab, enter the message you want to show in the email invitation that's sent to attendees and is shown on the event record.
    
    Optionally, you can get writing help for the **Message** field from our generative AI service, NetSuite Text Enhance. Click the **Enhance Text** button to use the available options. For more information about using this capability, see [Text Enhance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2171112518.html).
    
5.  Click the **Attendees** subtab.
    
6.  In the **Send Invitation To** column, select a name from the list. For more information, see [Sending Event Invitations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N502840.html).
    
7.  In the **Attendance** column choose whether this attendee is required or optional.
    
8.  Click **Add**.
    
9.  Repeat these steps for each attendee.
    
10.  On the **Resources** subtab, you can reserve the necessary resources for this event such as a conference room or presentation materials. For more information, see [Reserving Resources for Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N503835.html).
     
     You can see the availability of the people and materials you've selected on the **Attendees** or **Resources** subtabs on the **Availability** subtab.
     
     Click the arrows next to the date to view the availability on other days. The time window shown on this subtab is the same as the Daily start and end times set in your calendar preferences.
     
11.  Click the **Recurrence** subtab if the event is part of a series of events. For more information, see [Setting Up Recurring Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N503084.html).
     
12.  When you've finished entering all of the information for this event, click **Save**.
     

The following are optional settings on the event record:

-   On the **Related Records** subtab:
    
    -   Select a company if this event is related to a customer, vendor, partner, or other name. The event record is attached to the entity record.
        
    -   The **Contact** field lists the contacts for the entity you've selected. Select the contact with whom this event is associated, if any.
        
    -   If this event pertains to a support case, select the case number in the Support Case field. The event record is attached to the case record.
        
    -   If this event is related to a transaction, select the transaction number. The event is listed on the **Events** subtab of the transaction record.
        
-   Use the **Time Tracking** subtab, if you use the Time Tracking for CRM feature and want to track time for this event. For more information, see [Tracking Time for Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N503967.html).
    
-   Click the **Communication** subtab to attach a file to this event. For more information about how to attach files, see [Attaching Files to Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N490137.html).
    

### Additional Information

-   [Setting Calendar Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N500263.html)

### Related Topics

-   [Scheduling Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N501467.html)
-   [Using the Event Scheduler Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N502460.html)
-   [Event Scheduling Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N502623.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
