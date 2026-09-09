---
id: "section_N2638981"
type: "section"
title: "Delete Web Site Redirects Mass Update"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > SEO & Analytics > Search Engine Optimization (SEO) > SEO and Redirects > Delete Web Site Redirects Mass Update"
parent: "section_N2637891"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2638981.html"
anchors: ["procedure_N2638997"]
sha256: "023fecb7facfff21703b38c9b74f0fced2d308d41db7fdb22dd6c80b8c26ec79"
---

If you have the Mass Updates permission, you can use the Mass Updates feature to delete multiple redirect records simultaneously. When you set up this kind of mass update, you enter criteria for which redirects you want to delete. The system shows you a list of records that match, and then you can delete them right away or save the mass update definition for later. If you've got the Schedule Mass Updates permission, you can also schedule a mass update to run regularly.

#### To define a mass update that deletes URL redirects in bulk: {#procedure_N2638997}

1.  Go to Lists > Mass Update > Mass Updates.
    
2.  In the **Mass Updates** list, expand **Web Site Redirects**, and click **Delete Web Site Redirects**.
    
3.  In the **Title of Action** field, enter a name for this update.
    
4.  On the **Criteria** subtab, select a filter for finding the redirect records to be deleted.
    
    For information, see [Advanced Search Criteria Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646477.html).
    
5.  (Optional) On the **Results** subtab, define display options for the Mass Update Preview page that lists redirect records to be deleted.
    
    For information, see [Search Results Display Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648053.html).
    
6.  (Optional) On the **Audience** subtab, if available, define the users who can run the update.
    
7.  (Optional) If you are an administrator and you want to run the mass update on a recurring basis, set up this recurrence on the **Schedule** subtab. See [Scheduling a Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668529.html).
    
8.  Click **Preview** to review the records to be changed.
    
9.  Choose one of the following options:
    
    -   Click **Perform Update** to delete the records.
        
        Warning:
        
        After you click Perform Update, you cannot stop or cancel the mass update, so proceed with caution!
        
    -   Click **Save** to save this mass update for future use.
        
        -   When you save the update, it is not run. The mass update is saved with the search filters you have selected to find records that should be deleted. When you run the mass update in the future, it uses these search filters and lets you preview the list of returned records before performing the delete.
            
        -   To run a saved mass update, go to Lists > Mass Update > Saved Mass Updates, and click **Preview** next to the name of the update. On the Mass Update Preview page, click **Perform Update**.
            

For more information, see [Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1103335211.html).

### Related Topics

-   [Setting Up a URL Redirect](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2638072.html)
-   [Updating Redirect Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2638305.html)
-   [Importing Website Redirects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2638492.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
