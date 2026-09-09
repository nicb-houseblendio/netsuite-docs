---
id: "section_N1868140"
type: "section"
title: "Colombia Tax Setup"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Colombia Tax Topics > Colombia Tax Setup"
parent: "chapter_N1867954"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1868140.html"
anchors: ["bridgehead_N1868233", "bridgehead_N1868852", "bridgehead_N1869335", "bridgehead_N1871077"]
sha256: "d3eae089db06f8365a002edaf39aac99d8299383e6bdec2bbf4659f3f473b618"
---

For guidance on setting up your NetSuite account to track and report taxes in Colombia, read the following topics:

-   [Account Settings for Colombia](#bridgehead_N1868233)
    
-   [Colombia Tax Control Accounts](#bridgehead_N1868852)
    
-   [Colombia Tax Types](#bridgehead_N1869335)
    
-   [Colombia Tax Preferences](#bridgehead_N1871077)
    
-   [Colombia Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1871228.html)
    

## Account Settings for Colombia {#bridgehead_N1868233}

The following are suggested settings for Colombia:

1.  Setup > Company > Company Information
    
    -   Country: Colombia
        
    -   Time Zone: GMT -500 hours
        
    -   Currency format: Colombian Peso $1.234,56
        
2.  Setup > Company > Enable Features
    
    Check Multiple Currencies
    
3.  Setup > Company > General Preferences
    
    -   Date Format: DD/MM/YYYY
        
    -   Long Date Format: DD Month YYYY
        
    -   Time Format: hh:mm AM/PM
        
    -   Do not check the box for Use State Abbreviations in Addresses
        
4.  Setup > Company > Printing & Fax
    
    Do not check the box for Print Business Number on Forms
    
5.  Setup > Company > Accounting Preferences
    
    Check Use Account Numbers
    
6.  Lists > Accounting > Currencies
    
    Base currency: Colombian Peso (COP)
    
7.  Lists > Relationships > Vendors
    
    Default tax collection agency: Direccion de Impuestos y Aduanas Nacionales
    
8.  Setup > Company > States/Provinces/Counties
    

| Amazonas | Choco | Putumayo |
| --- | --- | --- |
| Antioquia | Cordoba | Quindio |
| Arauca | Cundinamarca | Risaralda |
| Atlantico | Guainia | San Andres, Providencia |
| Bolivar | Guaviare | Santander |
| Boyaca | Huila | Sucre |
| Caldas | La Guajira | Tolima |
| Caqueta | Magdalena | Valle del Cauca |
| Casanare | Meta | Vaupes |
| Cauca | Nariño | Vichada |
| Cesar | Norte de Santander | Bogota Capital District |

## Colombia Tax Control Accounts {#bridgehead_N1868852}

To create a tax control account, go to Setup > Accounting > Taxes > Tax Control Accounts > New. Use the following tax control accounts for Colombia:

| Tax Control Account Name | Tax Account Type |
| --- | --- |
| IVA on Purchases at 16% CO | Purchase |
| IVA on Purchases at 5% CO | Purchase |
| IVA on Sales at 16% CO | Sale |
| IVA on Sales at 5% CO | Sale |

## Colombia Tax Types {#bridgehead_N1869335}

To create a tax type, go to Setup > Accounting > Taxes > Tax Types > New. Use the following tax types for Colombia

| Tax Type | Liability/Sales Tax Account | Asset/Purchase Tax Account |
| --- | --- | --- |
| IVA\_CO | IVA on Sales at 16% CO | IVA on Purchases at 16% CO |
| IVA5\_CO | IVA on Sales at 5% CO | IVA on Purchases at 5% CO |

## Colombia Tax Preferences {#bridgehead_N1871077}

To set tax preferences, go to Setup > Accounting > Set Up Taxes. Use the following preferences for Colombia:

-   Tax Code for International Sale: X-CO
    
-   Default Tax Code: S-CO
    
-   Tax Rounding Method: Round Off
    

For information about setting up tax codes for Colombia, see [Colombia Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1871228.html).

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Colombia Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1871228.html)
-   [Setting Up Tax Filing for Colombia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3788090444.html)
-   [Colombia VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1872768.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
