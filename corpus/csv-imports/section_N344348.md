---
id: "section_N344348"
type: "section"
title: "Select a File for Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Step One Scan & Upload File > Select a File for Import"
parent: "section_N343532"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344348.html"
anchors: []
sha256: "fd5c2e419832425bf4481896955ba4e5a86a21fbef8fb78e54ec820aaaf36af5"
---

On the Scan & Upload CSV File page, choose the file or files you want to import.

For some record types, an option button is available to indicate whether you want to upload one or multiple files. There is a limit of 25,000 records per uploaded file.

Choose one or more CSV files to import by clicking the **Select...** buttons and browsing to the CSV files you want to import.

-   If you have chosen One file to upload, you'll see only one **Select...** button.
    
-   If you have chosen Multiple files to upload, you'll have a **Select...** button for the primary file, and multiple, optional **Select...** buttons with descriptions of the types of files that can be linked to the primary file.
    
    It is important that the data for the main fields in the imported records is included in the primary file, not in the linked files.
    
    Linked files may contain sublist or subrecord data that is stored separately, such as multiple addresses for each customer. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html). To avoid errors, make sure each file matches the right structure: sublist files should only have sublist fields, and subrecord files should only have subrecord fields.
    

Click the Select buttons for the data you want to upload, and browse to the correct files. After you've added a file, its name appears. You can click the Remove button to select a different file.

Important:

If you need to edit or rename a file after selecting it, you must remove it and add it again after the changes. If you change the file after selecting it and click Next, you'll get an error message.

The following screenshot shows file selection for a multi-file import:

![Example of a multiple files import in Step 1.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/MultFileImp.png)

Note the following:

-   The list of optional linked files shows sublists you may be able to import. It doesn't update if features are disabled, so you might see sublists that aren't currently available.
    
-   If you select multiple files, the Import Assistant's File Mapping page requires you to define the column in each file that links the data together.
    

Important:

If you are using a previously saved import map, your choice of one file or multiple files should be consistent with the original choice for the import map. If you choose one file for a map that previously used multiple files, or the reverse, some CSV file data may not be imported.

### Related Topics

-   [Step One Scan & Upload File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N343532.html)
-   [Select an Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N343713.html)
-   [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html)
-   [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html)
-   [Choose CSV Column Delimiter](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4341195935.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
