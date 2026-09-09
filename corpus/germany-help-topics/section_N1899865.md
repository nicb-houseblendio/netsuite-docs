---
id: "section_N1899865"
type: "section"
title: "What goes into each box - Germany Monthly/Quarterly VAT report"
branch: "germany-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Germany Help Topics > Germany Tax Topics For Accounts Without SuiteTax > Germany VAT Report > What goes into each box - Germany Monthly/Quarterly VAT report"
parent: "section_N1899458"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1899865.html"
anchors: []
sha256: "eec2856a2fbe1d27b42f3f8530c0a8af5ff932d940664818200fd43ec8485ae9"
---

Note:

Nondeductible tax codes created by checking the **100% Non-deductible** box on the Tax Code page isn't supported. If you want to create nondeductible tax codes that will work with International Tax Reports SuiteApp, see [Setting Up Nondeductible Input Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1822730.html).

The following table shows how NetSuite uses the tax codes to get the values for the Preliminary VAT return (monthly/quarterly report) for Germany. For annual VAT returns, see [What goes into each box - Germany Annual VAT Declaration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1905036.html).

| Line | English Label | Etiqueta Alemana | Box | Assessment basis without sales tax EUR | Box | Tax EUR ct |
| --- | --- | --- | --- | --- | --- | --- |
|  | **A. Taxable supplies, other services and gratuitous value deliveries** | **A. Steuerpflichtige Lieferungen, sonstige Leistungen und unentgeltliche Wertabgaben** |  |  |  |  |
|  | **Taxable Transactions** | **Steuerplichtige Umsätze** |  |  |  |  |
| 12 | at the tax rate of 19% | zum Steuersatz von 19 % | 81 | Net amount of sales S-DE | 81b | Tax amount of sales S-DE + Tax amount of sales adjustment in box 81b with S-DE |
| 13 |  |  | 86 | Net amount of sales R-DE | 86b | Tax amount of sales R-DE + Tax amount of sales adjustment in box 86b with R-DE |
| 14 | at the tax rate of 0% | zum Steuersatz von 0 % | 87 | Net amount of sales ZR-DE |  |  |
| 15 | to other tax rates | zu anderen Steuersätzen | 35 | Net amount of sales SR-DE, S2-DE, R1-DE | 36 | Tax amount of sales SR-DE, S2-DE, R1-DE + Tax amount of sales adjustment in box 36 with SR-DE, S2-DE, R1-DE |
| 16 | Deliveries of agricultural and forestry operations according to § 24 UStG to customers with sales tax Identification Number | Lieferungen land- und forstwirtschaftlicher Betriebe nach § 24 UStG an Abnehmer **mit** Umsatzsteuer-Identifikationsnummer | 77 | Editable field |  |  |
| 17 | Sales for which a tax is payable according to § 24 UStG (Sawmill products, beverages and alcoholic liquids, e.g. wine) | Umsätze, für die eine Steuer nach § 24 UStG zu entrichtenist (Sägewerkserzeugnisse, Getränke und alkoholische Flüs -sigkeiten, z. B. Wein) | 76 | Editable field | 80 | Editable field |
|  | **B. Tax-free deliveries, other services and free valuables** | **B. Steuerfreie Lieferungen, sonstige Leistungen und unentgeltliche Wertabgaben** |  |  |  |  |
|  | **Tax-free transactions with input VAT deduction** | **Steuerfreie Umsätze mit Vorsteuerabzug** |  |  |  |  |
|  | **Intra-community deliveries** (§ 4 No. 1 letter b UStG) | **Innergemeinschaftliche Lieferungen**(§ 4 Nummer 1 Buchstabe b UStG) |  |  |  |  |
| 18 | to buyers with a sales tax identification number | an Abnehmer **mit** Umsatzsteuer-Identifikationsnummer | 41 | Net amount of sales ES-DE, EZ-DE, ER-DE, ES1-DE, ER1-DE | \- | \- |
| 19 | new vehicles to buyers without sales tax Identification Number | neuer Fahrzeuge an Abnehmer **ohne** Umsatzsteuer-Identifikationsnummer | 44 | Editable field | \- | \- |
| 20 | new vehicles outside of a company (§ 2a UStG) | neuer Fahrzeuge außerhalb eines Unternehmens(§ 2a UStG) | 49 | Editable field | \- | \- |
| 21 | **Further tax-free sales with input tax deduction** (e.g. export deliveries, sales according to § 4 No. 2 to 7 UStG) | **Weitere steuerfreie Umsätze mit Vorsteuerabzug** z. B. **Ausfuhrlieferungen**, Umsätze nach § 4 Nummer 2 bis 7 UStG | 43 | Net amount of sales ZX-DE, E-DE | \- | \- |
| 22 | **Tax-free sales without input tax deduction** (e.g. sales according to § 4 No. 8 to 29 UStG) | **Steuerfreie Umsätze ohne Vorsteuerabzug** z. B. Umsätze nach § 4 Nummer 8 bis 29 UStG | 48 | Net amount of sales Z-DE | \- | \- |
|  | **C. Intra-Community Acquisitions** | **C. Innergemeinschaftliche Erwerbe** |  |  |  |  |
| 23 | **Tax-free intra-community acquisitions** of certain objects and gold investment (§§ 4b and 25c UStG) | **Steuerfreie innergemeinschaftliche Erwerbe** von bestimmten Gegenständen und Anlagegold(§§ 4b und 25c UStG) | 91 | Net amount of purchases EZ-DE | \- | \- |
| 24 | Taxable intra-community acquisitions at a tax rate of 19% | Steuerpflichtige innergemeinschaftliche Erwerbe zum Steuersatz von 19 % | 89 | Net amount of purchases ES-DE, EST-DE | 89b | Notional tax amount of purchases ES-DE + tax amount EST-DE |
| 25 | at a tax rate of 7% | zum Steuersatz von 7 % | 93 | Net amount of purchases ER-DE, ERT-DE | 93b | Notional tax amount of purchases ER-DE + tax amount ERT-DE |
| 26 | at the rate of 0% | zum Steuersatz von 0 % | 90 | Net amount of purchases EZR-DE |  |  |
| 27 | to other tax rates | zu anderen Steuersätzen | 95 | Net amount of purchases ESR-DE if applied notional rate is greater than 0% Net amount of purchases ES1-DE and ER1-DE | 98 | Notional amount of purchases ESR-DE, ES1-DE, ER1-DE |
| 28 | new vehicles (§ 1b paragraph 2 and 3 UStG) from suppliers without a sales tax identification number in general tax rate | **neuer Fahrzeuge** (§ 1b Absatz 2 und 3 UStG) von Lieferern **ohne** Umsatzsteuer-Identifikationsnummer zum allgemeinen Steuersatz | 94 | Editable field | 96 | Editable field |
|  | **D. Service recipient as tax debtor (§ 13b UStG)** | **D. Leistungsempfänger als Steuerschuldner(§ 13b UStG)** |  |  |  |  |
| 29 | Other services according to § 3a paragraph 2 UStG of an entrepreneur based in the rest of the community (§ 13b paragraph 1 UStG) | Sonstige Leistungen nach § 3a Absatz 2 UStG eines im übrigen Gemeinschaftsgebiet ansässigen Unternehmers(§ 13b Absatz 1 UStG) | 46 | Net amount of purchases ESSP-DE, ESSP1-DE | 47 | Notional amount of purchases ESSP-DE, ESSP1-DE |
| 30 | Sales that fall under the GrEStG (Section 13b paragraph 2 No. 3 UStG) | Umsätze, die unter das GrEStG fallen(§ 13b Absatz 2 Nummer 3 UStG) | 73 | Editable field | 74 | Editable field |
| 31 | Other services (§ 13b paragraph 2 No. 1, 2, 4 to 12 UStG) | Andere Leistungen(§ 13b Absatz 2 Nummer 1, 2, 4 bis 12 UStG) | 84 | Net amount of purchases S1-DE, RC-DE, IS-DE, SS1-DE, RC1-DE, IS1-DE | 85 | Notional amount of purchases S1-DE, RC-DE, IS-DE, SS1-DE, RC1-DE, IS1-DE + Tax amount of purchases IS-DE |
|  | **E. Additional information on sales** | **E. Ergänzende Angaben zu Umsätzen** |  |  |  |  |
| 32 | Deliveries by the first customer in intra-community triangular transactions (§ 25b UStG) | Lieferungen des ersten Abnehmers bei **innergemeinschaftlichen Dreiecksgeschäften** (§ 25b UStG) | 42 | Editable field | \- | \- |
| 33 | Taxable sales of the performing entrepreneur for which the service recipient pays the tax according to § 13b paragraph 5 UStG | Steuerpflichtige Umsätze des leistenden Unternehmers, fürdie der **Leistungsempfänger** die **Steuer nach § 13bAbsatz 5 UStG schuldet** | 60 | Net amount of sales S1-DE, RC-DE, SS1-DE, RC1-DE | \- | \- |
| 34 | **Non taxable supply of services** according to § 18b sentence 1 no. 2 UStG | **Nicht steuerbare sonstige Leistungen** gemäß § 18b Satz 1Nummer 2 UStG | 21 | Net amount of sales ESSS-DE, ESSS1-DE, ESSP-DE | \- | \- |
| 35 | **Other non-taxable transactions** (place of supply outside Germany) | **Übrige nicht steuerbare Umsätze** (Leistungsort nicht im Inland) | 45 | Net amount of sales OS-DE | \- | \- |
| 36 | **VAT (total of lines 12 to 17 and 24 to 31)** | **Umsatzsteuer (Summe der Zeilen 12 bis 17 und 24 bis 31)** |  |  |  |  |
|  | **F. Deductible Input Tax Amounts and Adjustment of Input Tax Deduction** | **F. Abziehbare Vorsteuerbeträge und Berichtigung des Vorsteuerabzugs** |  |  |  |  |
| 37 | Input tax amounts from invoices from other companies (§ 15paragraph 1 sentence 1 number 1 UStG), from services within the meaning of § 13a paragraph 1 number 6 UStG (§ 15 paragraph1 sentence 1 number 5 UStG) and from intra-community - chentriangular transactions (§ 25b paragraph 5 UStG) | Vorsteuerbeträge aus Rechnungen von anderen Unternehmern (§ 15 Absatz 1 Satz 1 Nummer 1 UStG), aus Leistungen im Sinne des § 13a Absatz 1 Nummer 6 UStG (§ 15 Absatz 1 Satz 1 Nummer 5 UStG) und aus innergemeinschaftlichen Dreiecksgeschäften (§ 25b Absatz 5 UStG) | \- | \- | 66 | Tax amount of purchases R-DE, S-DE, R1-DE, S1-DE + Deduct TAX amount for R-DE, S-DE, R1-DE, S2-DE - NonDeduct TAX amount for R-DE, S-DE, R1-DE, S2-DE + Tax amount of purchases adjustment in box 66 with R-DE, S-DE, R1-DE, S2-DE |
| 38 | Input tax amounts from the intra-community acquisition of items (§ 15 paragraph 1 sentence 1 number 3 UStG) | Vorsteuerbeträge aus dem innergemeinschaftlichen Erwerbvon Gegenständen(§ 15 Absatz 1 Satz 1 Nummer 3 UStG) | \- | \- | 61 | Box 89B + Box 93B + Box 98 |
| 39 | Import sales tax incurred (§ 15paragraph 1 sentence 1 number 2 UStG) | Entstandene Einfuhrumsatzsteuer(§ 15 Absatz 1 Satz 1 Nummer 2 UStG) | \- | \- | 62 | Net amount of purchases IT-DE |
| 40 | Input tax amounts from services within the meaning of § 13bUStG (§ 15 paragraph 1 sentence 1 number 4 UStG) | Vorsteuerbeträge aus Leistungen im Sinne des § 13b UStG(§ 15 Absatz 1 Satz 1 Nummer 4 UStG) | \- | \- | 67 | Notional amount of purchases ESSP-DE, IS-DE, RC-DE, S1-DE, ESSP1-DE, IS1-DE, RC1-DE, SS1-DE |
| 41 | Input tax calculated according to the general average rates (§ 23a UStG) | Vorsteuerbeträge, die nach allgemeinen Durchschnittssätzenberechnet sind (§ 23a UStG) | \- | \- | 63 | Editable field |
| 42 | Input tax deduction for intra-community deliveries of new vehicles outside of a company (§ 2a UStG) and small businesses within the meaning of § 19 paragraph1 UStG (§ 15 paragraph 4a UStG) | Vorsteuerabzug für innergemeinschaftliche Lieferungenneuer Fahrzeuge außerhalb eines Unternehmens(§ 2a UStG) sowie von Kleinunternehmern im Sinne des§ 19 Absatz 1 UStG (§ 15 Absatz 4a UStG) | \- | \- | 59 | Editable field |
| 43 | Correction of input tax deduction (§ 15a UStG) | Berichtigung des Vorsteuerabzugs (§ 15a UStG) | \- | \- | 64 | Editable field |
| 44 | Remaining amount (Line 36 minus lines 37 to 43) | Verbleibender Betrag(Zeile 36 abzüglich der Zeilen 37 bis 43) |  |  |  | Line 36 - Box 66 - Box 61 - Box 62 - Box 67 - Box 63 - Box 59 - Box 64 |
|  | **G. Other Tax Amounts** | **G. Andere Steuerbeträge** |  |  |  |  |
| 45 | Tax as a result of the change in the form of taxation as well as Additional tax on taxed advance payments and the like due to a change in tax rate | Steuer infolge des Wechsels der Besteuerungsform sowieNachsteuer auf versteuerte Anzahlungen und ähnlichemwegen Steuersatzänderung | \- | \- | 65 | Editable field |
| 46 | Tax amounts incorrectly or unjustifiably shown on invoices (§ 14c UStG) as well as tax amounts according to§ 6a paragraph 4 sentence 2, § 17 paragraph 1 sentence 7,§ 25b paragraph 2 UStG or from a outsourcer or warehouse keeper according to § 13a paragraph 1 number 6 UStG | In Rechnungen unrichtig oder unberechtigt ausgewieseneSteuerbeträge (§ 14c UStG) sowie Steuerbeträge, die nach§ 6a Absatz 4 Satz 2, § 17 Absatz 1 Satz 7, § 25b Absatz 2UStG oder von einem Auslagerer oder Lagerhalter nach§ 13a Absatz 1 Nummer 6 UStG geschuldet werden | \- | \- | 69 | Editable field |
|  | **H. Prepayment/Excess** | **H.Vorauszahlung/Überschuss** |  |  |  |  |
| 47 | **Sales tax prepayment / surplus** **(sum of lines 44 to 46)** | **Umsatzsteuer-Vorauszahlung/Überschuss** **(Summe der Zeilen 44 bis 46)** |  |  |  | Line 44 + box 65 + box 69 |
| 48 | Deduction of the specified special advance payment for a permanent extension of the deadline (usually only to be completed in the last advance notification of the taxation period) | **Abzug** der festgesetzten **Sondervorauszahlung** für Dauerfristverlängerung(in der Regel nur in der letzten Voranmeldung des Besteuerungszeitraums auszufüllen) |  |  | 39 | Editable field |
| 49 | **Remaining sales tax prepayment** **Remaining surplus** - please precede the amount with a minus - **(Please fill out in any case)** | **Verbleibende Umsatzsteuer-Vorauszahlung** Verbleibender **Überschuss** - bitte dem Betrag ein Minusvoranstellen - **(Bitte in jedem Fall ausfüllen)** |  |  | 83 | Line 44 + Box 65 + Box 69 - Box 39 |
|  | **I. Additional information on reductions accordingto § 17 paragraph 1 sentences 1 and 2 in connectionwith paragraph 2 number 1 sentence 1 UStG** | **I. Ergänzende Angaben zu Minderungen nach§ 17 Absatz 1 Sätze 1 und 2 in Verbindung mitAbsatz 2 Nummer 1 Satz 1 UStG** |  |  |  |  |
| 50 | Reduction of the tax base (included in rows 12 to 17) | Minderung der Bemessungsgrundlage(in den Zeilen 12 bis 17 enthalten) | 50 | Editable field |  |  |
| 51 | Reduction of the deductible input tax amounts (contained in line 37 from invoices from other entrepreneurs (§ 15 paragraph 1 Sentence 1 No. 1 UtG) as well as in lines 41 and 42) | Minderung der abziehbaren Vorsteuerbeträge(in der Zeile 37 aus Rechnungen von anderen Unternehmen(§ 15 Absatz 1 Satz 1 Nummer 1 UStG) sowie in den Zeilen 41 und 42 enthalten) |  |  | 37 | Editable field |

### Additional Information

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [VAT and GST Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2050963.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

### Related Topics

-   [What goes into each box - Germany Annual VAT Declaration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1905036.html)
-   [Germany VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1899458.html)
-   [Germany Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1897828.html)
-   [Setting Up Tax Filing for Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1917361.html)
-   [Submission of VAT Returns in Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1917621.html)
-   [Recapitulative Statement (EU Sales List) for Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1918495.html)
-   [Intrastat Report for Germany](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4149981058.html)
-   [Germany GoBD Data Export](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3838969498.html)
-   [Germany Tax Topics For Accounts Without SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554981475.html)
-   [Germany Account Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554726737.html)
-   [Setting Up Germany-Specific Preferences Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554726820.html)
-   [Germany-specific SuiteApps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158529777788.html)
-   [Germany Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554985535.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
