---
id: "section_N2070438"
type: "section"
title: "Commodity Code"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > European Union (EU) Tax Topics > EU Intrastat Report > Intrastat Reporting Fields > Commodity Code"
parent: "section_4150707116"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2070438.html"
anchors: []
sha256: "03f8e44f8d98bfb5c641098fa9d2e6f26a7accb43ad54b61e1908e0d136c321a"
---

The commodity code is the most important field on the Supplementary Declaration (SD). It's the basis for most of the statistical information used by government departments, the European Commission, United Nations agencies and businesses.

Each year, the European Commission publishes an updated list of commodity codes to reflect changes in international tariff and statistical nomenclature. You need the correct commodity code to file an Intrastat report. This eight-digit number identifies the type of goods in a Dispatch or Arrival declaration. See [European Commission's Combined Nomenclature](https://ec.europa.eu/taxation_customs/business/calculation-customs-duties/customs-tariff/combined-nomenclature_en) page for more information.

Note:

For some EU subsidiaries, you can enter up to 10 digits in the Commodity Code field on an Item record.

NetSuite can generate an EU Intrastat Dispatch or Arrival declaration for any of your EU subsidiary if you've installed the International Tax Reports SuiteApp.

Enter the commodity code on the Tax Reporting subtab of the Item record. After you enter it, click the Commodity Code Validation link. The system tells you if it's valid, but only checks if the code exists in the Combined Nomenclature (CN). It doesn't check if the item and the code match. Be sure to assign the correct commodity code to the item. See the [European Commission's Combined Nomenclature](https://ec.europa.eu/taxation_customs/business/calculation-customs-duties/customs-tariff/combined-nomenclature_en) page for more information.

Note:

For Netherlands, you can enter up to 10 digits in the Commodity Code field on an Item record. But, only the first 8 digits appear on the report.

The Commodity Code field is available on the following Item types:

-   Inventory Item
    
    -   Lot Numbered Inventory Item
        
    -   Serialized Inventory Item
        
-   Non-inventory Item
    
-   Other Charge
    
-   Kit/Package
    

Important:

NetSuite treats a kit as a single line item in transactions. It can't be broken down into its member items with separate prices and commodity codes. If you want your Intrastat report to include all items, use Item Group instead of Kit/Package. For more information, see [Key Differences Between Kits, Groups, and Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2318089.html#subsect_163301236648).

### Related Topics:

-   [EU Intrastat Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2069213.html)
-   [EU Intrastat Report Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2069786.html)
-   [Intrastat Reporting Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4150707116.html)
-   [Intrastat Report Dispatches and Arrivals Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2070008.html)
-   [Nature of Transaction Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2070738.html)
-   [Delivery Terms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2071234.html)
-   [Mode of Transport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1505110665.html)
-   [Supplementary Unit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4605983594.html)
-   [Generating an EU Intrastat Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2071452.html)
-   [Intrastat Report for Austria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4587020795.html)
-   [Intrastat Report for Belgium](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1552962932.html)
-   [Intrastat Report for Denmark](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1505371864.html)
-   [Intrastat Report for Finland](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1504769975.html)
-   [France Intrastat Declaration of Exchange of Goods (DEB) Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157018267486.html)
-   [Intrastat Report for Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4149981058.html)
-   [Intrastat Report for Netherlands](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1503450407.html)
-   [Intrastat Report for United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2035309.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Creating or Customizing Roles to Use the International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054151.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
