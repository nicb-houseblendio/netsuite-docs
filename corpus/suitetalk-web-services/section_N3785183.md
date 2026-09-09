---
id: "section_N3785183"
type: "section"
title: "Country Enumerations"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Country, State, and Language Enumerations > Country Enumerations"
parent: "chapter_N3784994"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3785183.html"
anchors: []
sha256: "9c3838f4b9e68e31725e9f065a3e3dda7238419be849f7dc9341872c4c1c3fb1"
---

The following table lists countries, as defined in NetSuite dropdown lists, and the corresponding enumeration to be used when populating these fields in SOAP web services requests.

The country codes listed here are the ISO compliant country code string values returned when performing a search operation on entity records, whereas the schema enumeration is the corresponding value used during a request. These enumerations are also listed as common.xsd types in the [SOAP Schema Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/enum/country.html?mode=package).

These enumerations can be used for all standard country fields in SOAP web services operations. These enumerations do not work in SOAP web services operations on custom fields that reference a List/Record of Country. In these cases, the internal ID of the country (country code) must be used. The internal ID can be obtained by calling the [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) operation. This operation allows the creation of a mapping of country values with their internal IDs.

Note:

The countryofmanufacture field for an item must be a country covered by FedEx or UPS.

Note:

The code for Kosovo is not included in ISO 3166-1, so usually the user-assigned code XK is being used. User-assigned codes are not universal and may not be compatible between different entities.

| Country | Schema Enumeration | Country Code |
| --- | --- | --- |
| Afghanistan | \_afghanistan | AF |
| Åland Islands | \_alandIslands | AX |
| Albania | \_albania | AL |
| Algeria | \_algeria | DZ |
| American Samoa | \_americanSamoa | AS |
| Andorra | \_andorra | AD |
| Angola | \_angola | AO |
| Anguilla | \_anguilla | AI |
| Antarctica | \_antarctica | AQ |
| Antigua and Barbuda | \_antiguaAndBarbuda | AG |
| Argentina | \_argentina | AR |
| Armenia | \_armenia | AM |
| Aruba | \_aruba | AW |
| Australia | \_australia | AU |
| Austria | \_austria | AT |
| Azerbaijan | \_azerbaijan | AZ |
| Bahamas | \_bahamas | BS |
| Bahrain | \_bahrain | BH |
| Bangladesh | \_bangladesh | BD |
| Barbados | \_barbados | BB |
| Belarus | \_belarus | BY |
| Belgium | \_belgium | BE |
| Belize | \_belize | BZ |
| Benin | \_benin | BJ |
| Bermuda | \_bermuda | BM |
| Bhutan | \_bhutan | BT |
| Bolivia (Plurinational State of) | \_boliviaPlurinationalStateOf | BO |
| Bonaire, Sint Eustatius and Saba | \_bonaireSaintEustatiusAndSaba | BQ |
| Bosnia and Herzegovina | \_bosniaAndHerzegovina | BA |
| Botswana | \_botswana | BW |
| Bouvet Island | \_bouvetIsland | BV |
| Brazil | \_brazil | BR |
| British Indian Ocean Territory | \_britishIndianOceanTerritory | IO |
| Brunei Darussalam | \_bruneiDarussalam | BN |
| Bulgaria | \_bulgaria | BG |
| Burkina Faso | \_burkinaFaso | BF |
| Burundi | \_burundi | BI |
| Cabo Verde | \_caboVerde | CV |
| Cambodia | \_cambodia | KH |
| Cameroon | \_cameroon | CM |
| Canada | \_canada | CA |
| Canary Islands | \_canaryIslands | IC |
| Cayman Islands | \_caymanIslands | KY |
| Central African Republic | \_centralAfricanRepublic | CF |
| Ceuta and Melilla | \_ceutaAndMelilla | EA |
| Chad | \_chad | TD |
| Chile | \_chile | CL |
| China | \_china | CN |
| Christmas Island | \_christmasIsland | CX |
| Cocos (Keeling) Islands | \_cocosKeelingIslands | CC |
| Colombia | \_colombia | CO |
| Comoros | \_comoros | KM |
| Congo | \_congo | CG |
| Congo (the Democratic Republic of the) | \_congoTheDemocraticRepublicOfThe | CD |
| Cook Islands | \_cookIslands | CK |
| Costa Rica | \_costaRica | CR |
| Côte d'Ivoire | \_coteDIvoire | CI |
| Croatia | \_croatia | HR |
| Cuba | \_cuba | CU |
| Curacao | \_curacao | CW |
| Cyprus | \_cyprus | CY |
| Czechia | \_czechia | CZ |
| Denmark | \_denmark | DK |
| Djibouti | \_djibouti | DJ |
| Dominica | \_dominica | DM |
| Dominican Republic | \_dominicanRepublic | DO |
| Ecuador | \_ecuador | EC |
| Egypt | \_egypt | EG |
| El Salvador | \_elSalvador | SV |
| Equatorial Guinea | \_equatorialGuinea | GQ |
| Eritrea | \_eritrea | ER |
| Estonia | \_estonia | EE |
| Eswatini | \_eswatini | SZ |
| Ethiopia | \_ethiopia | ET |
| Falkland Islands (Malvinas) | \_falklandIslandsMalvinas | FK |
| Faroe Islands | \_faroeIslands | FO |
| Fiji | \_fiji | FJ |
| Finland | \_finland | FI |
| France | \_france | FR |
| French Guiana | \_frenchGuiana | GF |
| French Polynesia | \_frenchPolynesia | PF |
| French Southern Territories | \_frenchSouthernTerritories | TF |
| Gabon | \_gabon | GA |
| Gambia | \_gambia | GM |
| Georgia | \_georgia | GE |
| Germany | \_germany | DE |
| Ghana | \_ghana | GH |
| Gibraltar | \_gibraltar | GI |
| Greece | \_greece | GR |
| Greenland | \_greenland | GL |
| Grenada | \_grenada | GD |
| Guadeloupe | \_guadeloupe | GP |
| Guam | \_guam | GU |
| Guatemala | \_guatemala | GT |
| Guernsey | \_guernsey | GG |
| Guinea | \_guinea | GN |
| Guinea-Bissau | \_guineaBissau | GW |
| Guyana | \_guyana | GY |
| Haiti | \_haiti | HT |
| Heard Island and McDonald Islands | \_heardIslandAndMcDonaldIslands | HM |
| Holy See | \_holySee | VA |
| Honduras | \_honduras | HN |
| Hong Kong | \_hongKong | HK |
| Hungary | \_hungary | HU |
| Iceland | \_iceland | IS |
| India | \_india | IN |
| Indonesia | \_indonesia | ID |
| Iran (Islamic Republic of) | \_iranIslamicRepublicOf | IR |
| Iraq | \_iraq | IQ |
| Ireland | \_ireland | IE |
| Isle of Man | \_isleOfMan | IM |
| Israel | \_israel | IL |
| Italy | \_italy | IT |
| Jamaica | \_jamaica | JM |
| Japan | \_japan | JP |
| Jersey | \_jersey | JE |
| Jordan | \_jordan | JO |
| Kazakhstan | \_kazakhstan | KZ |
| Kenya | \_kenya | KE |
| Kiribati | \_kiribati | KI |
| Korea (the Democratic People's Republic of) | \_koreaTheDemocraticPeoplesRepublicOf | KP |
| Korea (the Republic of) | \_koreaTheRepublicOf | KR |
| Kosovo | \_kosovo | XK |
| Kuwait | \_kuwait | KW |
| Kyrgyzstan | \_kyrgyzstan | KG |
| Lao, People's Democratic Republic | \_laoPeoplesDemocraticRepublic | LA |
| Latvia | \_latvia | LV |
| Lebanon | \_lebanon | LB |
| Lesotho | \_lesotho | LS |
| Liberia | \_liberia | LR |
| Libya | \_libya | LY |
| Liechtenstein | \_liechtenstein | LI |
| Lithuania | \_lithuania | LT |
| Luxembourg | \_luxembourg | LU |
| Macao | \_macao | MO |
| Madagascar | \_madagascar | MG |
| Malawi | \_malawi | MW |
| Malaysia | \_malaysia | MY |
| Maldives | \_maldives | MV |
| Mali | \_mali | ML |
| Malta | \_malta | MT |
| Marshall Islands | \_marshallIslands | MH |
| Martinique | \_martinique | MQ |
| Mauritania | \_mauritania | MR |
| Mauritius | \_mauritius | MU |
| Mayotte | \_mayotte | YT |
| Mexico | \_mexico | MX |
| Micronesia (Federated States of) | \_micronesiaFederalStatesOf | FM |
| Moldova (the Republic of) | \_moldovaTheRepublicOf | MD |
| Monaco | \_monaco | MC |
| Mongolia | \_mongolia | MN |
| Montenegro | \_montenegro | ME |
| Montserrat | \_montserrat | MS |
| Morocco | \_morocco | MA |
| Mozambique | \_mozambique | MZ |
| Myanmar | \_myanmar | MM |
| Namibia | \_namibia | NA |
| Nauru | \_nauru | NR |
| Nepal | \_nepal | NP |
| Netherlands | \_netherlands | NL |
| New Caledonia | \_newCaledonia | NC |
| New Zealand | \_newZealand | NZ |
| Nicaragua | \_nicaragua | NI |
| Niger | \_niger | NE |
| Nigeria | \_nigeria | NG |
| Niue | \_niue | NU |
| Norfolk Island | \_norfolkIsland | NF |
| Northern Mariana Islands | \_northernMarianaIslands | MP |
| North Macedonia | \_northMacedonia | MK |
| Norway | \_norway | NO |
| Oman | \_oman | OM |
| Pakistan | \_pakistan | PK |
| Palau | \_palau | PW |
| Palestine (State of) | \_palestineStateOf | PS |
| Panama | \_panama | PA |
| Papua New Guinea | \_papuaNewGuinea | PG |
| Paraguay | \_paraguay | PY |
| Peru | \_peru | PE |
| Philippines | \_philippines | PH |
| Pitcairn | \_pitcairn | PN |
| Poland | \_poland | PL |
| Portugal | \_portugal | PT |
| Puerto Rico | \_puertoRico | PR |
| Qatar | \_qatar | QA |
| Réunion | \_reunion | RE |
| Romania | \_romania | RO |
| Russian Federation | \_russianFederation | RU |
| Rwanda | \_rwanda | RW |
| Saint Barthélemy | \_saintBarthelemy | BL |
| Saint Helena, Ascension and Tristan da Cunha | \_saintHelenaAscensionAndTristanDaCunha | SH |
| Saint Kitts and Nevis | \_saintKittsAndNevis | KN |
| Saint Lucia | \_saintLucia | LC |
| Saint Martin (French part) | \_saintMartinFrenchPart | MF |
| Saint Pierre and Miquelon | \_saintPierreAndMiquelon | PM |
| Saint Vincent and the Grenadines | \_saintVincentAndTheGrenadines | VC |
| Samoa | \_samoa | WS |
| San Marino | \_sanMarino | SM |
| Sao Tome and Principe | \_saoTomeAndPrincipe | ST |
| Saudi Arabia | \_saudiArabia | SA |
| Senegal | \_senegal | SN |
| Serbia | \_serbia | RS |
| Seychelles | \_seychelles | SC |
| Sierra Leone | \_sierraLeone | SL |
| Singapore | \_singapore | SG |
| Sint Maarten (Dutch part) | \_sintMaartenDutchPart | SX |
| Slovakia | \_slovakia | SK |
| Slovenia | \_slovenia | SI |
| Solomon Islands | \_solomonIslands | SB |
| Somalia | \_somalia | SO |
| South Africa | \_southAfrica | ZA |
| South Georgia and the South Sandwich Islands | \_southGeorgiaAndTheSouthSandwichIslands | GS |
| South Sudan | \_southSudan | SS |
| Spain | \_spain | ES |
| Sri Lanka | \_sriLanka | LK |
| Sudan | \_sudan | SD |
| Suriname | \_suriname | SR |
| Svalbard and Jan Mayen | \_svalbardAndJanMayen | SJ |
| Sweden | \_sweden | SE |
| Switzerland | \_switzerland | CH |
| Syrian Arab Republic | \_syrianArabRepublic | SY |
| Taiwan (Province of China) | \_taiwan | TW |
| Tajikistan | \_tajikistan | TJ |
| Tanzania, the United Republic of | \_tanzaniaTheUnitedRepublicOf | TZ |
| Thailand | \_thailand | TH |
| Timor-Leste | \_timorLeste | TL |
| Togo | \_togo | TG |
| Tokelau | \_tokelau | TK |
| Tonga | \_tonga | TO |
| Trinidad and Tobago | \_trinidadAndTobago | TT |
| Tunisia | \_tunisia | TN |
| Türkiye | \_turkiye | TR |
| Turkmenistan | \_turkmenistan | TM |
| Turks and Caicos Islands | \_turksAndCaicosIslands | TC |
| Tuvalu | \_tuvalu | TV |
| Uganda | \_uganda | UG |
| Ukraine | \_ukraine | UA |
| United Arab Emirates | \_unitedArabEmirates | AE |
| United Kingdom | \_unitedKingdom | GB |
| United States | \_unitedStates | US |
| United States Minor Outlying Islands | \_unitedStatesMinorOutlyingIslands | UM |
| Uruguay | \_uruguay | UY |
| Uzbekistan | \_uzbekistan | UZ |
| Vanuatu | \_vanuatu | VU |
| Venezuela (Bolivarian Republic of) | \_venezuelaBolivarianRepublicOf | VE |
| Viet Nam | \_vietnam | VN |
| Virgin Islands (British) | \_virginIslandsBritish | VG |
| Virgin Islands (U.S.) | \_virginIslandsUS | VI |
| Wallis and Futuna Islands | \_wallisAndFutunaIslands | WF |
| Western Sahara | \_westernSahara | EH |
| Yemen | \_yemen | YE |
| Zambia | \_zambia | ZM |
| Zimbabwe | \_zimbabwe | ZW |

### Related Topics

-   [Country, State, and Language Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3784994.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
