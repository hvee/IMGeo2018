# Objecttypen

De objecttypen worden hieronder besproken.

# Objecttype: IMGeo-Object

| **Naam objecttype**               | IMGeo-Object                                                                                                                                                                                                                                                                                                                                                                                                               |
|-----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<ADEElement\>\> \<\<BGT\>\> \<\<objecttype\>\>                                                                                                                                                                                                                                                                                                                                                                          |
| **Herkomst objecttype**           | BGT                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Code objecttype**               | 10                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Definitie objecttype**          | De gemeenschappelijke eigenschappen van een grootschalig topografisch object, al dan niet uit de basisregistratie.                                                                                                                                                                                                                                                                                                         |
| **Herkomst definitie objecttype** | BGT                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Datum opname objecttype**       |                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Subtype van**                   | \_CityObject                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Toelichting objecttype**        |                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Unieke aanduiding objecttype**  | Identificatie                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Populatie**                     |                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Kwaliteitsbegrip**              |                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Overzicht associaties**         |                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Overzicht attributen**          | \<\<BGT\>\>objectBeginTijd [1-1]<br />\<\<BGT\>\>objectEindTijd [0-1]<br />\<\<BGT\>\>identificatie [1-1]<br />\<\<BGT\>\>tijdstipRegistratie [1-1]<br />\<\<BGT\>\>eindRegistratie [0-1]<br />\<\<BGT\>\>LV-publicatiedatum [0-1]<br />\<\<BGT\>\>bronhouder [1-1]<br />\<\<BGT\>\>inOnderzoek [1-1]<br />\<\<BGT\>\>relatieveHoogteligging [1-1]<br />\<\<BGT\>\>status [1-1]<br />plus-status [0-1] |

# Objecttype: Wegdeel

| **Naam objecttype**               | Wegdeel                                                                                                                                                                                                   |
|-----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<ADEElement\>\> \<\<BGT\>\> \<\<objecttype\>\>                                                                                                                                                         |
| **Herkomst objecttype**           | BGT                                                                                                                                                                                                       |
| **Code objecttype**               | 20                                                                                                                                                                                                        |
| **Definitie objecttype**          | Kleinste functioneel onafhankelijk stukje van een NEN 3610 Weg met gelijkblijvende, homogene eigenschappen en relaties en primair bedoeld voor gebruik door weg-, spoor- en vliegverkeer te land.         |
| **Herkomst definitie objecttype** | BGT                                                                                                                                                                                                       |
| **Datum opname objecttype**       |                                                                                                                                                                                                           |
| **Subtype van**                   | TrafficArea                                                                                                                                                                                               |
| **Toelichting objecttype**        |                                                                                                                                                                                                           |
| **Unieke aanduiding objecttype**  | Identificatie                                                                                                                                                                                             |
| **Populatie**                     |                                                                                                                                                                                                           |
| **Kwaliteitsbegrip**              |                                                                                                                                                                                                           |
| **Overzicht associaties**         | \<\<BGT\>\>kruinlijnWegdeel [0..1]<br />\<\<BGT\>\>geometrie2dWegdeel [1..1]<br />lod0SurfaceWegdeel [0..1]                                                                                           |
| **Overzicht attributen**          | \<\<BGT\>\>bgt-functie [1-1]<br />\<\<BGT\>\>bgt-fysiekVoorkomen [1-1]<br />plus-functieWegdeel [0-1]<br />\<\<BGT\>\>\<\<voidable\>\>wegdeelOpTalud [1-1]<br />plus-fysiekVoorkomenWegdeel [0-1] |

# Objecttype: OndersteunendWegdeel

| **Naam objecttype**               | OndersteunendWegdeel                                                                                                                                                                                                                             |
|-----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<ADEElement\>\> \<\<BGT\>\> \<\<objecttype\>\>                                                                                                                                                                                                |
| **Herkomst objecttype**           | BGT                                                                                                                                                                                                                                              |
| **Code objecttype**               | 70                                                                                                                                                                                                                                               |
| **Definitie objecttype**          | Een deel van de weg dat niet primair bedoeld is voor gebruik door het verkeer.                                                                                                                                                                   |
| **Herkomst definitie objecttype** | CityGML                                                                                                                                                                                                                                          |
| **Datum opname objecttype**       |                                                                                                                                                                                                                                                  |
| **Subtype van**                   | AuxiliaryTrafficArea                                                                                                                                                                                                                             |
| **Toelichting objecttype**        |                                                                                                                                                                                                                                                  |
| **Unieke aanduiding objecttype**  | Identificatie.                                                                                                                                                                                                                                   |
| **Populatie**                     |                                                                                                                                                                                                                                                  |
| **Kwaliteitsbegrip**              |                                                                                                                                                                                                                                                  |
| **Overzicht associaties**         | \<\<BGT\>\>geometrie2dOndersteunendWegdeel [1..1]<br />lod0SurfaceOndersteunendWegdeel [0..1]<br />\<\<BGT\>\>kruinlijnOndersteunendWegdeel [0..1]                                                                                           |
| **Overzicht attributen**          | \<\<BGT\>\>bgt-functie [1-1]<br />\<\<BGT\>\>bgt-fysiekVoorkomen [1-1]<br />\<\<BGT\>\>\<\<voidable\>\>ondersteunendWegdeelOpTalud [1-1]<br />plus-functieOndersteunendWegdeel [0-1]<br />plus-fysiekVoorkomenOndersteunendWegdeel [0-1] |

# Objecttype: Spoor

| **Naam objecttype**               | Spoor                                                                                                                                          |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<ADEElement\>\> \<\<BGT\>\> \<\<objecttype\>\>                                                                                              |
| **Herkomst objecttype**           | BGT                                                                                                                                            |
| **Code objecttype**               | 100                                                                                                                                            |
| **Definitie objecttype**          | De as van het spoor, dat wil zeggen het midden van twee stalen staven op een onderling vaste afstand, waarover trein, tram, of sneltram rijdt. |
| **Herkomst definitie objecttype** | IMGeo 1.0                                                                                                                                      |
| **Datum opname objecttype**       |                                                                                                                                                |
| **Subtype van**                   | Railway                                                                                                                                        |
| **Toelichting objecttype**        |                                                                                                                                                |
| **Unieke aanduiding objecttype**  | Identificatie                                                                                                                                  |
| **Populatie**                     |                                                                                                                                                |
| **Kwaliteitsbegrip**              |                                                                                                                                                |
| **Overzicht associaties**         | lod0CurveSpoor [0..1]<br />\<\<BGT\>\>geometrie2dSpoor [1..1]                                                                                |
| **Overzicht attributen**          | \<\<BGT\>\>bgt-functie [1-1]<br />plus-functieSpoor [0-1]                                                                                    |

# Objecttype: OnbegroeidTerreindeel

| **Naam objecttype**               | OnbegroeidTerreindeel                                                                                                                                              |
|-----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<featureType\>\> \<\<BGT\>\> \<\<objecttype\>\>                                                                                                                 |
| **Herkomst objecttype**           | BGT                                                                                                                                                                |
| **Code objecttype**               | 30                                                                                                                                                                 |
| **Definitie objecttype**          | Kleinste functioneel onafhankelijk stukje van een terrein, dat er binnen het objecttype Terrein van NEN 3610 wordt onderscheiden, zonder aaneengesloten vegetatie. |
| **Herkomst definitie objecttype** | BGT                                                                                                                                                                |
| **Datum opname objecttype**       |                                                                                                                                                                    |
| **Subtype van**                   | LandUse                                                                                                                                                            |
| **Toelichting objecttype**        |                                                                                                                                                                    |
| **Unieke aanduiding objecttype**  | Identificatie                                                                                                                                                      |
| **Populatie**                     | Alle vlakken die geen vegetatie bedekking hebben en geen (ondersteunend) wegdeel, waterdeel of bouwwerk zijn.                                                      |
| **Kwaliteitsbegrip**              |                                                                                                                                                                    |
| **Overzicht associaties**         | \<\<BGT\>\>kruinlijnOnbegroeidTerreindeel [0..1]<br />\<\<BGT\>\>geometrie2dOnbegroeidTerreindeel [1..1]                                                         |
| **Overzicht attributen**          | \<\<BGT\>\>bgt-fysiekVoorkomen [1-1]<br />\<\<BGT\>\>\<\<voidable\>\>onbegroeidTerreindeelOpTalud [1-1]<br />plus-fysiekVoorkomen [0-1]                        |

# Objecttype: BegroeidTerreindeel

| **Naam objecttype**               | BegroeidTerreindeel                                                                                                                                            |
|-----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<ADEElement\>\> \<\<BGT\>\> \<\<objecttype\>\>                                                                                                              |
| **Herkomst objecttype**           | BGT                                                                                                                                                            |
| **Code objecttype**               | 140                                                                                                                                                            |
| **Definitie objecttype**          | Kleinste functioneel onafhankelijk stukje van een terrein dat er binnen het objecttype Terrein van NEN 3610 wordt onderscheiden, met aaneengesloten vegetatie. |
| **Herkomst definitie objecttype** | BGT                                                                                                                                                            |
| **Datum opname objecttype**       |                                                                                                                                                                |
| **Subtype van**                   | PlantCover                                                                                                                                                     |
| **Toelichting objecttype**        | Vlakvormig groenobject.                                                                                                                                        |
| **Unieke aanduiding objecttype**  | identificatie.                                                                                                                                                 |
| **Populatie**                     |                                                                                                                                                                |
| **Kwaliteitsbegrip**              |                                                                                                                                                                |
| **Overzicht associaties**         | lod0MultiSurfaceBegroeidTerreindeel [0..1]<br />\<\<BGT\>\>geometrie2dBegroeidTerreindeel [1..1]<br />\<\<BGT\>\>kruinlijnBegroeidTerreindeel [0..1]       |
| **Overzicht attributen**          | \<\<BGT\>\>bgt-fysiekVoorkomen [1-1]<br />\<\<BGT\>\>\<\<voidable\>\>begroeidTerreindeelOpTalud [1-1]<br />plus-fysiekVoorkomen [0-1]                      |

# Objecttype: Waterdeel

| **Naam objecttype**               | Waterdeel                                                                                                                                                                                                         |
|-----------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<objecttype\>\> \<\<BGT\>\> \<\<featureType\>\>                                                                                                                                                                |
| **Herkomst objecttype**           | BGT                                                                                                                                                                                                               |
| **Code objecttype**               | 40                                                                                                                                                                                                                |
| **Definitie objecttype**          | Kleinste functioneel onafhankelijk stukje water met gelijkblijvende, homogene eigenschappen en relaties dat er binnen het objecttype Water van NEN 3610 wordt onderscheiden en dat permanent met water bedekt is. |
| **Herkomst definitie objecttype** | BGT                                                                                                                                                                                                               |
| **Datum opname objecttype**       |                                                                                                                                                                                                                   |
| **Subtype van**                   | WaterBody                                                                                                                                                                                                         |
| **Toelichting objecttype**        |                                                                                                                                                                                                                   |
| **Unieke aanduiding objecttype**  | Identificatie                                                                                                                                                                                                     |
| **Populatie**                     |                                                                                                                                                                                                                   |
| **Kwaliteitsbegrip**              |                                                                                                                                                                                                                   |
| **Overzicht associaties**         | \<\<BGT\>\>geometrie2dWaterdeel [1..1]                                                                                                                                                                            |
| **Overzicht attributen**          | \<\<BGT\>\>bgt-type [1-1]<br />plus-type [0-1]                                                                                                                                                                  |

# Objecttype: OndersteunendWaterdeel

| **Naam objecttype**               | OndersteunendWaterdeel                                                                                |
|-----------------------------------|-------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<objecttype\>\> \<\<BGT\>\> \<\<featureType\>\>                                                    |
| **Herkomst objecttype**           | BGT                                                                                                   |
| **Code objecttype**               | 41                                                                                                    |
| **Definitie objecttype**          | Object dat in het kader van de waterhuishouding periodiek gedeeltelijk of geheel met water is bedekt. |
| **Herkomst definitie objecttype** | BGT                                                                                                   |
| **Datum opname objecttype**       |                                                                                                       |
| **Subtype van**                   | WaterBody                                                                                             |
| **Toelichting objecttype**        |                                                                                                       |
| **Unieke aanduiding objecttype**  | Identificatie.                                                                                        |
| **Populatie**                     |                                                                                                       |
| **Kwaliteitsbegrip**              |                                                                                                       |
| **Overzicht associaties**         | \<\<BGT\>\>geometrie2dOndersteunendWaterdeel [1..1]                                                   |
| **Overzicht attributen**          | \<\<BGT\>\>bgt-type [1-1]<br />plus-type [0-1]                                                      |

# Objecttype: Pand

| **Naam objecttype**               | Pand                                                                                                                                                                                         |
|-----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<ADEElement\>\> \<\<BGT\>\> \<\<objecttype\>\>                                                                                                                                            |
| **Herkomst objecttype**           | BAG                                                                                                                                                                                          |
| **Code objecttype**               | 60                                                                                                                                                                                           |
| **Definitie objecttype**          | Een PAND is de kleinste bij de totstandkoming functioneel en bouwkundig-constructief zelfstandige eenheid die direct en duurzaam met de aarde is verbonden en betreedbaar en afsluitbaar is. |
| **Herkomst definitie objecttype** | Stelselcatalogus                                                                                                                                                                             |
| **Datum opname objecttype**       |                                                                                                                                                                                              |
| **Subtype van**                   | BuildingPart                                                                                                                                                                                 |
| **Toelichting objecttype**        |                                                                                                                                                                                              |
| **Unieke aanduiding objecttype**  | Identificatie                                                                                                                                                                                |
| **Populatie**                     | Zie BAG                                                                                                                                                                                      |
| **Kwaliteitsbegrip**              |                                                                                                                                                                                              |
| **Overzicht associaties**         | \<\<BGT\>\>geometrie2dGrondvlak [1..1]                                                                                                                                                       |
| **Overzicht attributen**          | \<\<BGT\>\>identificatieBAGPND [1-1]<br />\<\<BGT\>\>nummeraanduidingreeks [0-\*]                                                                                                          |

# Objecttype: OverigeConstructie

| **Naam objecttype**               | OverigeConstructie                                                                                                                                                                                                                                                                                                              |
|-----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<featureType\>\> \<\<BGT\>\> \<\<objecttype\>\>                                                                                                                                                                                                                                                                              |
| **Herkomst objecttype**           | BGT                                                                                                                                                                                                                                                                                                                             |
| **Code objecttype**               | 50                                                                                                                                                                                                                                                                                                                              |
| **Definitie objecttype**          | Abstract objecttype zijnde een gebouwd object dat niet valt onder de definitie van NEN 3610 Gebouw.                                                                                                                                                                                                                             |
| **Herkomst definitie objecttype** | BGT                                                                                                                                                                                                                                                                                                                             |
| **Datum opname objecttype**       |                                                                                                                                                                                                                                                                                                                                 |
| **Subtype van**                   | \_Site                                                                                                                                                                                                                                                                                                                          |
| **Toelichting objecttype**        | Deze klasse komt overeen met OtherConstruction in het Inspire Buildings thema.                                                                                                                                                                                                                                                  |
| **Unieke aanduiding objecttype**  | Identificatie                                                                                                                                                                                                                                                                                                                   |
| **Populatie**                     |                                                                                                                                                                                                                                                                                                                                 |
| **Kwaliteitsbegrip**              |                                                                                                                                                                                                                                                                                                                                 |
| **Overzicht associaties**         | \<\<BGT\>\>geometrie2dOverigeConstructie [1..1]<br />lod0Geometry [0..1]<br />lod1Geometry [0..1]<br />lod2Geometry [0..1]<br />lod3Geometry [0..1]<br />lod0ImplicitRepresentation [0..1]<br />lod1ImplicitRepresentation [0..1]<br />lod2ImplicitRepresentation [0..1]<br />lod3ImplicitRepresentation [0..1] |
| **Overzicht attributen**          |                                                                                                                                                                                                                                                                                                                                 |

# Objecttype: OverigBouwwerk

| **Naam objecttype**               | OverigBouwwerk                                                                                         |
|-----------------------------------|--------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<featureType\>\> \<\<BGT\>\> \<\<objecttype\>\>                                                     |
| **Herkomst objecttype**           | BGT                                                                                                    |
| **Code objecttype**               | 53                                                                                                     |
| **Definitie objecttype**          | Met de aarde verbonden duurzaam bouwwerk, dat niet valt onder de definities van een pand of kunstwerk. |
| **Herkomst definitie objecttype** | BGT                                                                                                    |
| **Datum opname objecttype**       |                                                                                                        |
| **Subtype van**                   | OverigeConstructie                                                                                     |
| **Toelichting objecttype**        | Een Overig Bouwwerk heeft in de BGT altijd vlakgeometrie. Een overkapping heeft multivlakgeometrie.    |
| **Unieke aanduiding objecttype**  | Identificatie.                                                                                         |
| **Populatie**                     |                                                                                                        |
| **Kwaliteitsbegrip**              |                                                                                                        |
| **Overzicht associaties**         |                                                                                                        |
| **Overzicht attributen**          | \<\<BGT\>\>bgt-type [1-1]<br />plus-type [0-1]                                                       |

# Objecttype: Overbruggingsdeel

| **Naam objecttype**               | Overbruggingsdeel                                                                                                                                                   |
|-----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<ADEElement\>\> \<\<BGT\>\> \<\<objecttype\>\>                                                                                                                   |
| **Herkomst objecttype**           | BGT                                                                                                                                                                 |
| **Code objecttype**               | 55                                                                                                                                                                  |
| **Definitie objecttype**          | Onderdeel van een beweegbare of vaste verbinding tussen twee punten, die door water, een weg of anderszins gescheiden zijn, dat essentieel is voor de constructie . |
| **Herkomst definitie objecttype** | BGT                                                                                                                                                                 |
| **Datum opname objecttype**       |                                                                                                                                                                     |
| **Subtype van**                   | BridgeConstructionElement                                                                                                                                           |
| **Toelichting objecttype**        |                                                                                                                                                                     |
| **Unieke aanduiding objecttype**  | Identificatie                                                                                                                                                       |
| **Populatie**                     |                                                                                                                                                                     |
| **Kwaliteitsbegrip**              |                                                                                                                                                                     |
| **Overzicht associaties**         | lod0GeometrieOverbruggingsdeel [0..1]<br />\<\<BGT\>\>geometrie2dOverbruggingsdeel [1..1]                                                                         |
| **Overzicht attributen**          | typeOverbruggingsdeel [0-1]<br />hoortBijTypeOverbrugging [0-1]<br />overbruggingIsBeweegbaar [0-1]                                                             |

# Objecttype: Tunneldeel

| **Naam objecttype**               | Tunneldeel                                                                                                 |
|-----------------------------------|------------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<ADEElement\>\> \<\<BGT\>\> \<\<objecttype\>\>                                                          |
| **Herkomst objecttype**           | BGT                                                                                                        |
| **Code objecttype**               | 56                                                                                                         |
| **Definitie objecttype**          | Onderdeel van een kunstmatig aangelegde, kokervormige onderdoorgang dat essentieel is voor de constructie. |
| **Herkomst definitie objecttype** | BGT                                                                                                        |
| **Datum opname objecttype**       |                                                                                                            |
| **Subtype van**                   | TunnelPart                                                                                                 |
| **Toelichting objecttype**        |                                                                                                            |
| **Unieke aanduiding objecttype**  | Identificatie                                                                                              |
| **Populatie**                     |                                                                                                            |
| **Kwaliteitsbegrip**              |                                                                                                            |
| **Overzicht associaties**         | \<\<BGT\>\>geometrie2dTunneldeel [1..1]<br />lod0GeometrieTunneldeel [0..1]                              |
| **Overzicht attributen**          |                                                                                                            |

# Objecttype: Kunstwerkdeel

| **Naam objecttype**               | Kunstwerkdeel                                                                                                               |
|-----------------------------------|-----------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<featureType\>\> \<\<BGT\>\> \<\<objecttype\>\>                                                                          |
| **Herkomst objecttype**           | BGT                                                                                                                         |
| **Code objecttype**               | 51                                                                                                                          |
| **Definitie objecttype**          | Onderdeel van een civiel-technisch werk voor de infrastructuur van wegen, water, spoorbanen, waterkeringen en/of leidingen. |
| **Herkomst definitie objecttype** | IMGeo 1.0                                                                                                                   |
| **Datum opname objecttype**       |                                                                                                                             |
| **Subtype van**                   | OverigeConstructie                                                                                                          |
| **Toelichting objecttype**        |                                                                                                                             |
| **Unieke aanduiding objecttype**  | Identificatie.                                                                                                              |
| **Populatie**                     |                                                                                                                             |
| **Kwaliteitsbegrip**              |                                                                                                                             |
| **Overzicht associaties**         |                                                                                                                             |
| **Overzicht attributen**          | \<\<BGT\>\>bgt-type [1-1]<br />plus-type [0-1]                                                                            |

# Objecttype: Scheiding

| **Naam objecttype**               | Scheiding                                                     |
|-----------------------------------|---------------------------------------------------------------|
| **Stereotype**                    | \<\<featureType\>\> \<\<BGT\>\> \<\<objecttype\>\>            |
| **Herkomst objecttype**           | BGT                                                           |
| **Code objecttype**               | 52                                                            |
| **Definitie objecttype**          | Kunstmatig, meestal lineair obstakel met een werende functie. |
| **Herkomst definitie objecttype** | BGT                                                           |
| **Datum opname objecttype**       |                                                               |
| **Subtype van**                   | OverigeConstructie                                            |
| **Toelichting objecttype**        |                                                               |
| **Unieke aanduiding objecttype**  | Identificatie.                                                |
| **Populatie**                     |                                                               |
| **Kwaliteitsbegrip**              |                                                               |
| **Overzicht associaties**         |                                                               |
| **Overzicht attributen**          | \<\<BGT\>\>bgt-type [1-1]<br />plus-type [0-1]              |

# Objecttype: OngeclassificeerdObject

| **Naam objecttype**               | OngeclassificeerdObject                                                                                                                                                                                                                                                     |
|-----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<featureType\>\> \<\<objecttype\>\> \<\<BGT\>\>                                                                                                                                                                                                                          |
| **Herkomst objecttype**           | BGT                                                                                                                                                                                                                                                                         |
| **Code objecttype**               | 900                                                                                                                                                                                                                                                                         |
| **Definitie objecttype**          | Object waarvoor geen bronhouder aangewezen is en/of dat niet nader is geclassificeerd.                                                                                                                                                                                      |
| **Herkomst definitie objecttype** | BGT                                                                                                                                                                                                                                                                         |
| **Datum opname objecttype**       |                                                                                                                                                                                                                                                                             |
| **Subtype van**                   | \_CityObject, IMGeo-Object                                                                                                                                                                                                                                                  |
| **Toelichting objecttype**        | Bedoeld voor objecten waarvoor geen BGT bronhouder is, zoals slivers tussen sloot en akker, natuurterreinen, sloten niet op de legger, terrein waar niemand toegang toe heeft, etc. Het object doet mee in de topologische structuur en komt alleen voor op maaiveldniveau. |
| **Unieke aanduiding objecttype**  | Identificatie.                                                                                                                                                                                                                                                              |
| **Populatie**                     |                                                                                                                                                                                                                                                                             |
| **Kwaliteitsbegrip**              |                                                                                                                                                                                                                                                                             |
| **Overzicht associaties**         | \<\<BGT\>\>geometrie2d [1..1]                                                                                                                                                                                                                                               |
| **Overzicht attributen**          |                                                                                                                                                                                                                                                                             |

# Objecttype: FunctioneelGebied

| **Naam objecttype**               | FunctioneelGebied                                                             |
|-----------------------------------|-------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<featureType\>\> \<\<BGT\>\> \<\<objecttype\>\>                            |
| **Herkomst objecttype**           | IMGeo 2.0                                                                     |
| **Code objecttype**               | 350                                                                           |
| **Definitie objecttype**          | Begrensd en benoemd gebied dat door een functionele eenheid beschreven wordt. |
| **Herkomst definitie objecttype** | BRT stelselcatalogus                                                          |
| **Datum opname objecttype**       |                                                                               |
| **Subtype van**                   | LandUse                                                                       |
| **Toelichting objecttype**        |                                                                               |
| **Unieke aanduiding objecttype**  | Identificatie.                                                                |
| **Populatie**                     |                                                                               |
| **Kwaliteitsbegrip**              |                                                                               |
| **Overzicht associaties**         | \<\<BGT\>\>geometrie2dFunctioneelGebied [1..1]                                |
| **Overzicht attributen**          | \<\<BGT\>\>bgt-type [1-1]<br />plus-type [0-1]<br />naam [0-1]            |

# Objecttype: OpenbareRuimteLabel

| **Naam objecttype**               | OpenbareRuimteLabel                                                                                                                                                                        |
|-----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<featureType\>\> \<\<BGT\>\> \<\<objecttype\>\>                                                                                                                                         |
| **Herkomst objecttype**           | BGT                                                                                                                                                                                        |
| **Code objecttype**               | 110                                                                                                                                                                                        |
| **Definitie objecttype**          | Naam en plaatsingspunten van een in de BAG geregistreerde OPENBARE RUIMTE.                                                                                                                 |
| **Herkomst definitie objecttype** | BGT                                                                                                                                                                                        |
| **Datum opname objecttype**       |                                                                                                                                                                                            |
| **Subtype van**                   | \_CityObject, IMGeo-Object                                                                                                                                                                 |
| **Toelichting objecttype**        | Dit objecttype wordt in de BGT geregistreerd ten behoeve van visualisatie-doeleinden. In het optionele IMGeo deel is het mogelijk ook de vlakgeometrie van de openbare ruimte op te nemen. |
| **Unieke aanduiding objecttype**  | Identificatie                                                                                                                                                                              |
| **Populatie**                     |                                                                                                                                                                                            |
| **Kwaliteitsbegrip**              |                                                                                                                                                                                            |
| **Overzicht associaties**         |                                                                                                                                                                                            |
| **Overzicht attributen**          | \<\<BGT\>\>identificatieBAGOPR [1-1]<br />\<\<BGT\>\>openbareRuimteNaam [1-1]<br />\<\<BGT\>\>openbareRuimteType [1-1]                                                                 |

# Objecttype: Plaatsbepalingspunt

| **Naam objecttype**               | Plaatsbepalingspunt                                                                                                                                                                                                                |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                    | \<\<featureType\>\> \<\<BGT\>\> \<\<objecttype\>\>                                                                                                                                                                                 |
| **Herkomst objecttype**           | BGT                                                                                                                                                                                                                                |
| **Code objecttype**               | 120                                                                                                                                                                                                                                |
| **Definitie objecttype**          | Punt dat is ingemeten en vervolgens gebruikt is bij en onderdeel uitmaakt van de begrenzing van BGT objecten.                                                                                                                      |
| **Herkomst definitie objecttype** | BGT                                                                                                                                                                                                                                |
| **Datum opname objecttype**       |                                                                                                                                                                                                                                    |
| **Subtype van**                   |                                                                                                                                                                                                                                    |
| **Toelichting objecttype**        | Dit objecttype wordt geregistreerd ten behoeve van kwaliteits-doeleinden.                                                                                                                                                          |
| **Unieke aanduiding objecttype**  | Identificatie                                                                                                                                                                                                                      |
| **Populatie**                     |                                                                                                                                                                                                                                    |
| **Kwaliteitsbegrip**              |                                                                                                                                                                                                                                    |
| **Overzicht associaties**         | \<\<BGT\>\>geometrie [1..1]                                                                                                                                                                                                        |
| **Overzicht attributen**          | \<\<BGT\>\>identificatie [1-1]<br />\<\<BGT\>\>\<\<voidable\>\>nauwkeurigheid [1-1]<br />\<\<BGT\>\>datumInwinning [1-1]<br />\<\<BGT\>\>\<\<voidable\>\>inwinnendeInstantie [1-1]<br />\<\<BGT\>\>inwinningsmethode [1-1] |

## Samengestelde attributen

### Nummeraanduidingreeks

| **Naam samengesteld attribuut**        | Nummeraanduidingreeks                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|----------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Definitie samengesteld attribuut**   | Samengesteld attribuut ten behoeve van opname van een reeks nummeraanduidingen van verblijfsobjecten in een pand.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Stereotype**                         | \<\<dataType\>\> \<\<BGT\>\> \<\<groepattribuuttype\>\>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Herkomst samengesteld attribuut**    | \-                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Toelichting samengesteld attribuut** | Uit de BAG afgeleide reeks nummeraanduidingen waarbij het laagste en hoogste bijbehorende huisnummer worden gevisualiseerd. Bij één pand kunnen meerdere reeksen nummeraanduidingen worden opgenomen (t.b.v galerijflats en dergelijke). In een reeks kunnen ook huisletters worden opgenomen. Bij een pand met één verblijfsobject wordt een nummeraanduidingreeks met daarin één huisnummer en eventueel huisletter en toevoeging opgenomen. De BAG identificatie van de verblijfsobjecten met het laagste en hoogste huisnummer wordt opgenomen. Als bij het pand maar één nummeraanduiding hoort, wordt de bijbehorende BAG identificatie opgenomen als laagste nummeraanduiding. Ten behoeve van visualisatie zijn het punt waar de nummeraanduidingreeks moet worden gevisualiseerd en eventueel de rotatiehoek opgenomen. |
| **Overzicht attributen**               | \<\<BGT\>\>nummeraanduidingreeks [1-1]<br />\<\<BGT\>\>identificatieBAGVBOLaagsteHuisnummer [1-1]<br />\<\<BGT\>\>identificatieBAGVBOHoogsteHuisnummer [0-1]                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |

### NEN3610ID

| **Naam samengesteld attribuut**        | NEN3610ID                                                                                                                                                                                                                       |
|----------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Definitie samengesteld attribuut**   | Identificatiegegevens voor de universeel unieke identificatie van een object.                                                                                                                                                   |
| **Stereotype**                         | \<\<dataType\>\> \<\<BGT\>\> \<\<groepattribuuttype\>\>                                                                                                                                                                         |
| **Herkomst samengesteld attribuut**    | \-                                                                                                                                                                                                                              |
| **Toelichting samengesteld attribuut** | De combinatie van namespace van een registratie, lokale identificatie en versie informatie maken een object uniek identificeerbaar. Met het NEN3610ID kun je daardoor met zekerheid verwijzen naar het geïdentificeerde object. |
| **Overzicht attributen**               | \<\<BGT\>\>namespace [1-1]<br />\<\<BGT\>\>lokaalID [1-1]                                                                                                                                                                     |

### Label

| **Naam samengesteld attribuut**        | Label                                                                                          |
|----------------------------------------|------------------------------------------------------------------------------------------------|
| **Definitie samengesteld attribuut**   | Een samengesteld attribuut voor verwijzing naar een te plaatsen labeltekst en positie daarvan. |
| **Stereotype**                         | \<\<dataType\>\> \<\<BGT\>\> \<\<groepattribuuttype\>\>                                        |
| **Herkomst samengesteld attribuut**    | \-                                                                                             |
| **Toelichting samengesteld attribuut** |                                                                                                |
| **Overzicht attributen**               | \<\<BGT\>\>tekst [1-1]<br />\<\<BGT\>\>positie [1-\*]                                        |

### Labelpositie

| **Naam samengesteld attribuut**        | Labelpositie                                                                                                               |
|----------------------------------------|----------------------------------------------------------------------------------------------------------------------------|
| **Definitie samengesteld attribuut**   | Locatie waar een label ten behoeve van visualisatie moet worden afgebeeld.                                                 |
| **Stereotype**                         | \<\<dataType\>\> \<\<BGT\>\> \<\<groepattribuuttype\>\>                                                                    |
| **Herkomst samengesteld attribuut**    | \-                                                                                                                         |
| **Toelichting samengesteld attribuut** | Ten behoeve van visualisatie is opgenomen het geometriepunt en eventuele rotatie die gewenst is bij het tonen van de naam. |
| **Overzicht attributen**               | \<\<BGT\>\>plaatsingspunt [1-1]<br />\<\<BGT\>\>hoek [1-1]                                                               |

# Beschrijving van de attributen en associaties

Hieronder worden de attributen van de BGT-objecttypen besproken. Alleen de voor
de BGT relevante attributen worden hier besproken. De overige attributen worden
in deel II, de Gegevenscatalogus IMGeo, toegelicht.

N.B. De objecten in dit hoofdstuk hebben een vaste volgorde. Deze volgorde geeft
een hiërarchie aan, die van belang is bij elkaar kruisende objecten, waarbij het
eerstgenoemde object de belangrijkste is.

IMGeo-Object
------------

### objectBeginTijd

| **Naam attribuut**               | objectBeginTijd                                                                                                     |
|----------------------------------|---------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<formeleLevensduur\>\> \<\<attribuuttype\>\>                                                         |
| **Herkomst attribuut**           | NEN 3610:2011                                                                                                       |
| **Code attribuut**               | 10.2                                                                                                                |
| **Definitie attribuut**          | Datum waarop het object bij de bronhouder is ontstaan.                                                              |
| **Waardetype attribuut**         | Date                                                                                                                |
| **Waardenverzameling**           |                                                                                                                     |
| **Multipliciteit**               | [1-1]                                                                                                               |
| **Datum opname**                 |                                                                                                                     |
| **Indicatie materiële historie** | Nee                                                                                                                 |
| **Indicatie formele historie**   | Ja                                                                                                                  |
| **Indicatie authentiek**         | Authentiek                                                                                                          |
| **Toelichting attribuut**        | Deze datum moet altijd gelijk zijn aan de datum uit de tijdstipregistratie van het eerste voorkomen van het object. |

### objectEindTijd

| **Naam attribuut**               | objectEindTijd                                                 |
|----------------------------------|----------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<formeleLevensduur\>\> \<\<attribuuttype\>\>    |
| **Herkomst attribuut**           | NEN 3610:2011                                                  |
| **Code attribuut**               | 10.3                                                           |
| **Definitie attribuut**          | Datum waarop het object bij de bronhouder niet meer geldig is. |
| **Waardetype attribuut**         | Date                                                           |
| **Waardenverzameling**           |                                                                |
| **Multipliciteit**               | [0-1]                                                          |
| **Datum opname**                 |                                                                |
| **Indicatie materiële historie** | Nee                                                            |
| **Indicatie formele historie**   | Ja                                                             |
| **Indicatie authentiek**         | Authentiek                                                     |
| **Toelichting attribuut**        |                                                                |

### identificatie

| **Naam attribuut**               | identificatie                                                                              |
|----------------------------------|--------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<identificatie\>\> \<\<attribuuttype\>\>                                    |
| **Herkomst attribuut**           | BGT                                                                                        |
| **Code attribuut**               | 10.1                                                                                       |
| **Definitie attribuut**          | Uniek identificatienummer voor het object dat onveranderlijk is zolang het object bestaat. |
| **Waardetype attribuut**         | NEN3610ID                                                                                  |
| **Waardenverzameling**           |                                                                                            |
| **Multipliciteit**               | [1-1]                                                                                      |
| **Datum opname**                 |                                                                                            |
| **Indicatie materiële historie** | Nee                                                                                        |
| **Indicatie formele historie**   | Nee                                                                                        |
| **Indicatie authentiek**         | Authentiek                                                                                 |
| **Toelichting attribuut**        | Zie 3.10 van de gegevenscatalogus.                                                         |

### tijdstipRegistratie

| **Naam attribuut**               | tijdstipRegistratie                                                                                                                                                                                              |
|----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<formeleHistorie\>\> \<\<attribuuttype\>\>                                                                                                                                                        |
| **Herkomst attribuut**           | NEN3610:2011                                                                                                                                                                                                     |
| **Code attribuut**               | 10.4                                                                                                                                                                                                             |
| **Definitie attribuut**          | Tijdstip waarop deze instantie van het object is opgenomen door de bronhouder.                                                                                                                                   |
| **Waardetype attribuut**         | DateTime                                                                                                                                                                                                         |
| **Waardenverzameling**           |                                                                                                                                                                                                                  |
| **Multipliciteit**               | [1-1]                                                                                                                                                                                                            |
| **Datum opname**                 |                                                                                                                                                                                                                  |
| **Indicatie materiële historie** | Nee                                                                                                                                                                                                              |
| **Indicatie formele historie**   | Ja                                                                                                                                                                                                               |
| **Indicatie authentiek**         | Authentiek                                                                                                                                                                                                       |
| **Toelichting attribuut**        | Als een mutatie niet resulteert in een nieuw object, dan ontstaat een nieuwe versie van het object. In deze situatie verandert het tijdstipRegistratie van het object, terwijl de objectBeginTijd gelijk blijft. |

### eindRegistratie

| **Naam attribuut**               | eindRegistratie                                                                                                                                        |
|----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<formeleHistorie\>\> \<\<attribuuttype\>\>                                                                                              |
| **Herkomst attribuut**           | NEN3610:2011                                                                                                                                           |
| **Code attribuut**               | 10.5                                                                                                                                                   |
| **Definitie attribuut**          | Eind van de periode waarop deze instantie van het object geldig is bij de bronhouder. Wanneer deze waarde niet is ingevuld is de instantie nog geldig. |
| **Waardetype attribuut**         | DateTime                                                                                                                                               |
| **Waardenverzameling**           |                                                                                                                                                        |
| **Multipliciteit**               | [0-1]                                                                                                                                                  |
| **Datum opname**                 |                                                                                                                                                        |
| **Indicatie materiële historie** | Nee                                                                                                                                                    |
| **Indicatie formele historie**   | Ja                                                                                                                                                     |
| **Indicatie authentiek**         | Authentiek                                                                                                                                             |
| **Toelichting attribuut**        |                                                                                                                                                        |

### LV-publicatiedatum

| **Naam attribuut**               | LV-publicatiedatum                                                                                                                                                                                                                                                    |
|----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                                                                                                                                                                                                     |
| **Herkomst attribuut**           | BGT                                                                                                                                                                                                                                                                   |
| **Code attribuut**               | 10.10                                                                                                                                                                                                                                                                 |
| **Definitie attribuut**          | Tijdstip waarop deze instantie van het object is opgenomen in de Landelijke Voorziening.                                                                                                                                                                              |
| **Waardetype attribuut**         | DateTime                                                                                                                                                                                                                                                              |
| **Waardenverzameling**           |                                                                                                                                                                                                                                                                       |
| **Multipliciteit**               | [0-1]                                                                                                                                                                                                                                                                 |
| **Datum opname**                 |                                                                                                                                                                                                                                                                       |
| **Indicatie materiële historie** | Nee                                                                                                                                                                                                                                                                   |
| **Indicatie formele historie**   | Ja                                                                                                                                                                                                                                                                    |
| **Indicatie authentiek**         | Authentiek                                                                                                                                                                                                                                                            |
| **Toelichting attribuut**        | Het gegeven is optioneel omdat een nieuw object pas een LV-publicatiedatum krijgt als het voor de eerste keer wordt opgenomen in de Landelijke Voorziening. Voor en tijdens aanlevering van een nieuw object aan de Landelijke Voorziening ontbreekt dit gegeven nog. |

### bronhouder

| **Naam attribuut**               | bronhouder                                                                                                                                                                                              |
|----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                                                                                                                                       |
| **Herkomst attribuut**           | BGT                                                                                                                                                                                                     |
| **Code attribuut**               | 10.6                                                                                                                                                                                                    |
| **Definitie attribuut**          | De bronhoudercode van het object.                                                                                                                                                                       |
| **Waardetype attribuut**         | CharacterString                                                                                                                                                                                         |
| **Waardenverzameling**           |                                                                                                                                                                                                         |
| **Multipliciteit**               | [1-1]                                                                                                                                                                                                   |
| **Datum opname**                 |                                                                                                                                                                                                         |
| **Indicatie materiële historie** | Nee                                                                                                                                                                                                     |
| **Indicatie formele historie**   | Ja                                                                                                                                                                                                      |
| **Indicatie authentiek**         | Authentiek                                                                                                                                                                                              |
| **Toelichting attribuut**        | Per object (dus niet per objecttype) moet de bronhouder worden vastgelegd zodat hiernaar kan worden gerefereerd bij terugmeldingen. Een object valt altijd geheel binnen het gebied van één bronhouder. |

### inOnderzoek

| **Naam attribuut**               | inOnderzoek                                                                                                                                       |
|----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                                                                                 |
| **Herkomst attribuut**           | Stelselcatalogus                                                                                                                                  |
| **Code attribuut**               | 10.7                                                                                                                                              |
| **Definitie attribuut**          | Een aanduiding waarmee wordt aangegeven dat een onderzoek wordt uitgevoerd naar de juistheid van een of meer gegevens van het betreffende object. |
| **Waardetype attribuut**         | Boolean                                                                                                                                           |
| **Waardenverzameling**           |                                                                                                                                                   |
| **Multipliciteit**               | [1-1]                                                                                                                                             |
| **Datum opname**                 |                                                                                                                                                   |
| **Indicatie materiële historie** | Nee                                                                                                                                               |
| **Indicatie formele historie**   | Ja                                                                                                                                                |
| **Indicatie authentiek**         | Authentiek                                                                                                                                        |
| **Toelichting attribuut**        |                                                                                                                                                   |

### relatieveHoogteligging

| **Naam attribuut**               | relatieveHoogteligging                             |
|----------------------------------|----------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                  |
| **Herkomst attribuut**           | BGT                                                |
| **Code attribuut**               | 10.8                                               |
| **Definitie attribuut**          | Aanduiding voor de relatieve hoogte van het object |
| **Waardetype attribuut**         | Integer                                            |
| **Waardenverzameling**           |                                                    |
| **Multipliciteit**               | [1-1]                                              |
| **Datum opname**                 |                                                    |
| **Indicatie materiële historie** | Nee                                                |
| **Indicatie formele historie**   | Ja                                                 |
| **Indicatie authentiek**         | Authentiek                                         |
| **Toelichting attribuut**        |                                                    |

### bgt-status

| **Naam attribuut**               | bgt-status                                                 |
|----------------------------------|------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                          |
| **Herkomst attribuut**           | IMGeo                                                      |
| **Code attribuut**               | 10.9                                                       |
| **Definitie attribuut**          | De status gekoppeld aan de levenscyclus van een geo-object |
| **Waardetype attribuut**         | GenericName                                                |
| **Waardenverzameling**           | Status                                                     |
| **Multipliciteit**               | [1-1]                                                      |
| **Datum opname**                 |                                                            |
| **Indicatie materiële historie** | Nee                                                        |
| **Indicatie formele historie**   | Ja                                                         |
| **Indicatie authentiek**         | Authentiek                                                 |
| **Toelichting attribuut**        | Default: bestaand                                          |

Wegdeel
-------

### bgt-functie

| **Naam attribuut**               | bgt-functie                                             |
|----------------------------------|---------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                       |
| **Herkomst attribuut**           | NEN 3610:2011                                           |
| **Code attribuut**               | 20.2                                                    |
| **Definitie attribuut**          | Specificatie van het hoofdgebruiksdoel van het wegdeel. |
| **Waardetype attribuut**         | GenericName                                             |
| **Waardenverzameling**           | FunctieWeg                                              |
| **Multipliciteit**               | [1-1]                                                   |
| **Datum opname**                 |                                                         |
| **Indicatie materiële historie** | Nee                                                     |
| **Indicatie formele historie**   | Ja                                                      |
| **Indicatie authentiek**         | Authentiek                                              |
| **Toelichting attribuut**        |                                                         |

### bgt-fysiekVoorkomen

| **Naam attribuut**               | bgt-fysiekVoorkomen                            |
|----------------------------------|------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>              |
| **Herkomst attribuut**           | BGT                                            |
| **Code attribuut**               | 20.3                                           |
| **Definitie attribuut**          | Mate waarin het wegdeel al of niet verhard is. |
| **Waardetype attribuut**         | GenericName                                    |
| **Waardenverzameling**           | FysiekVoorkomenWeg                             |
| **Multipliciteit**               | [1-1]                                          |
| **Datum opname**                 |                                                |
| **Indicatie materiële historie** | Nee                                            |
| **Indicatie formele historie**   | Ja                                             |
| **Indicatie authentiek**         | Authentiek                                     |
| **Toelichting attribuut**        |                                                |

### wegdeelOpTalud

| **Naam attribuut**               | wegdeelOpTalud                                                |
|----------------------------------|---------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\> \<\<voidable\>\>            |
| **Herkomst attribuut**           | BGT                                                           |
| **Code attribuut**               | 20.1                                                          |
| **Definitie attribuut**          | Indicatie of het object wel of niet op een hellend vlak ligt. |
| **Waardetype attribuut**         | Boolean                                                       |
| **Waardenverzameling**           |                                                               |
| **Multipliciteit**               | [1-1]                                                         |
| **Datum opname**                 | 21-11-2011                                                    |
| **Indicatie materiële historie** | Nee                                                           |
| **Indicatie formele historie**   | Ja                                                            |
| **Indicatie authentiek**         | Authentiek.                                                   |
| **Toelichting attribuut**        | Default: false (geen talud)                                   |

### Associatie: kruinlijnWegdeel

| **Definitie**      | Lijngeometrie van de hoogstgelegen begrenzing van een kunstmatig aangelegd en onderhouden helling. |
|--------------------|----------------------------------------------------------------------------------------------------|
| **Doelklasse**     | GM\_Curve                                                                                          |
| **Multipliciteit** | [0..1]                                                                                             |
| **Stereotype**     | \<\<BGT\>\> \<\<voidable\>\>                                                                       |
| **Toelichting**    |                                                                                                    |

### Associatie: geometrie2dWegdeel

| **Definitie**      | Vlakgeometrie. |
|--------------------|----------------|
| **Doelklasse**     | GM\_Surface    |
| **Multipliciteit** | [1..1]         |
| **Stereotype**     | \<\<BGT\>\>    |
| **Toelichting**    |                |

OndersteunendWegdeel
--------------------

### bgt-functie

| **Naam attribuut**               | bgt-functie                                                |
|----------------------------------|------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                          |
| **Herkomst attribuut**           | BGT                                                        |
| **Code attribuut**               | 70.1                                                       |
| **Definitie attribuut**          | Specificatie van de functie van het ondersteunend wegdeel. |
| **Waardetype attribuut**         | GenericName                                                |
| **Waardenverzameling**           | FunctieOndersteunendWegdeel                                |
| **Multipliciteit**               | [1-1]                                                      |
| **Datum opname**                 |                                                            |
| **Indicatie materiële historie** | Nee                                                        |
| **Indicatie formele historie**   | Ja                                                         |
| **Indicatie authentiek**         | Authentiek                                                 |
| **Toelichting attribuut**        |                                                            |

### bgt-fysiekVoorkomen

| **Naam attribuut**               | bgt-fysiekVoorkomen                                          |
|----------------------------------|--------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                            |
| **Herkomst attribuut**           | BGT                                                          |
| **Code attribuut**               | 70.3                                                         |
| **Definitie attribuut**          | Mate waarin het ondersteunend wegdeel al of niet verhard is. |
| **Waardetype attribuut**         | GenericName                                                  |
| **Waardenverzameling**           | FysiekVoorkomenOndersteunendWegdeel                          |
| **Multipliciteit**               | [1-1]                                                        |
| **Datum opname**                 | 28-11-2012                                                   |
| **Indicatie materiële historie** | Nee                                                          |
| **Indicatie formele historie**   | Ja                                                           |
| **Indicatie authentiek**         | Authentiek                                                   |
| **Toelichting attribuut**        |                                                              |

### ondersteunendWegdeelOpTalud

| **Naam attribuut**               | ondersteunendWegdeelOpTalud                                   |
|----------------------------------|---------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\> \<\<voidable\>\>            |
| **Herkomst attribuut**           | BGT                                                           |
| **Code attribuut**               | 70.2                                                          |
| **Definitie attribuut**          | Indicatie of het object wel of niet op een hellend vlak ligt. |
| **Waardetype attribuut**         | Boolean                                                       |
| **Waardenverzameling**           |                                                               |
| **Multipliciteit**               | [1-1]                                                         |
| **Datum opname**                 | 21-11-2011                                                    |
| **Indicatie materiële historie** | Nee                                                           |
| **Indicatie formele historie**   | Ja                                                            |
| **Indicatie authentiek**         | Authentiek.                                                   |
| **Toelichting attribuut**        | Default: false (geen talud)                                   |

### Associatie: geometrie2dOndersteunendWegdeel

| **Definitie**      | Vlakgeometrie. |
|--------------------|----------------|
| **Doelklasse**     | GM\_Surface    |
| **Multipliciteit** | [1..1]         |
| **Stereotype**     | \<\<BGT\>\>    |
| **Toelichting**    |                |

### Associatie: kruinlijnOndersteunendWegdeel

| **Definitie**      | Lijngeometrie van de hoogstgelegen begrenzing van een kunstmatig aangelegd en onderhouden helling. |
|--------------------|----------------------------------------------------------------------------------------------------|
| **Doelklasse**     | GM\_Curve                                                                                          |
| **Multipliciteit** | [0..1]                                                                                             |
| **Stereotype**     | \<\<BGT\>\> \<\<voidable\>\>                                                                       |
| **Toelichting**    |                                                                                                    |

Spoor
-----

### bgt-functie

| **Naam attribuut**               | bgt-functie                                       |
|----------------------------------|---------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\>                                       |
| **Herkomst attribuut**           | BGT                                               |
| **Code attribuut**               | 100.1                                             |
| **Definitie attribuut**          | Specificatie van het soort gebruik van het spoor. |
| **Waardetype attribuut**         | GenericName                                       |
| **Waardenverzameling**           | FunctieSpoor                                      |
| **Multipliciteit**               | [1-1]                                             |
| **Datum opname**                 |                                                   |
| **Indicatie materiële historie** | Nee                                               |
| **Indicatie formele historie**   | Ja                                                |
| **Indicatie authentiek**         | Authentiek                                        |
| **Toelichting attribuut**        |                                                   |

### Associatie: geometrie2dSpoor

| **Definitie**      | Lijngeometrie. |
|--------------------|----------------|
| **Doelklasse**     | GM\_Curve      |
| **Multipliciteit** | [1..1]         |
| **Stereotype**     | \<\<BGT\>\>    |
| **Toelichting**    |                |

OnbegroeidTerreindeel
---------------------

### bgt-fysiekVoorkomen

| **Naam attribuut**               | bgt-fysiekVoorkomen                                                                  |
|----------------------------------|--------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                    |
| **Herkomst attribuut**           | BGT                                                                                  |
| **Code attribuut**               | 30.1                                                                                 |
| **Definitie attribuut**          | Classificatie van het soort terrein, ingedeeld naar de uiterlijke verschijningsvorm. |
| **Waardetype attribuut**         | GenericName                                                                          |
| **Waardenverzameling**           | FysiekVoorkomenOnbegroeidTerrein                                                     |
| **Multipliciteit**               | [1-1]                                                                                |
| **Datum opname**                 |                                                                                      |
| **Indicatie materiële historie** | Nee                                                                                  |
| **Indicatie formele historie**   | Ja                                                                                   |
| **Indicatie authentiek**         | Authentiek                                                                           |
| **Toelichting attribuut**        |                                                                                      |

### onbegroeidTerreindeelOpTalud

| **Naam attribuut**               | onbegroeidTerreindeelOpTalud                                  |
|----------------------------------|---------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\> \<\<voidable\>\>            |
| **Herkomst attribuut**           | BGT                                                           |
| **Code attribuut**               | 30.2                                                          |
| **Definitie attribuut**          | Indicatie of het object wel of niet op een hellend vlak ligt. |
| **Waardetype attribuut**         | Boolean                                                       |
| **Waardenverzameling**           |                                                               |
| **Multipliciteit**               | [1-1]                                                         |
| **Datum opname**                 | 21-11-2011                                                    |
| **Indicatie materiële historie** | Nee                                                           |
| **Indicatie formele historie**   | Ja                                                            |
| **Indicatie authentiek**         | Authentiek.                                                   |
| **Toelichting attribuut**        | Default: false (geen talud)                                   |

### Associatie: kruinlijnOnbegroeidTerreindeel

| **Definitie**      | Lijngeometrie van de hoogstgelegen begrenzing van een kunstmatig aangelegd en onderhouden helling. |
|--------------------|----------------------------------------------------------------------------------------------------|
| **Doelklasse**     | GM\_Curve                                                                                          |
| **Multipliciteit** | [0..1]                                                                                             |
| **Stereotype**     | \<\<BGT\>\> \<\<voidable\>\>                                                                       |
| **Toelichting**    |                                                                                                    |

### Associatie: geometrie2dOnbegroeidTerreindeel

| **Definitie**      | Vlakgeometrie. |
|--------------------|----------------|
| **Doelklasse**     | GM\_Surface    |
| **Multipliciteit** | [1..1]         |
| **Stereotype**     | \<\<BGT\>\>    |
| **Toelichting**    |                |

BegroeidTerreindeel
-------------------

### bgt-fysiekVoorkomen

| **Naam attribuut**               | bgt-fysiekVoorkomen                                                 |
|----------------------------------|---------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                   |
| **Herkomst attribuut**           | BGT                                                                 |
| **Code attribuut**               | 140.1                                                               |
| **Definitie attribuut**          | Classificatie van het vegetatiedek, ingedeeld naar soort vegetatie. |
| **Waardetype attribuut**         | GenericName                                                         |
| **Waardenverzameling**           | FysiekVoorkomenBegroeidTerrein                                      |
| **Multipliciteit**               | [1-1]                                                               |
| **Datum opname**                 |                                                                     |
| **Indicatie materiële historie** | Nee                                                                 |
| **Indicatie formele historie**   | Ja                                                                  |
| **Indicatie authentiek**         | Authentiek                                                          |
| **Toelichting attribuut**        |                                                                     |

### begroeidTerreindeelOpTalud

| **Naam attribuut**               | begroeidTerreindeelOpTalud                                    |
|----------------------------------|---------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\> \<\<voidable\>\>            |
| **Herkomst attribuut**           | BGT                                                           |
| **Code attribuut**               | 140.2                                                         |
| **Definitie attribuut**          | Indicatie of het object wel of niet op een hellend vlak ligt. |
| **Waardetype attribuut**         | Boolean                                                       |
| **Waardenverzameling**           |                                                               |
| **Multipliciteit**               | [1-1]                                                         |
| **Datum opname**                 | 21-11-2011                                                    |
| **Indicatie materiële historie** | Nee                                                           |
| **Indicatie formele historie**   | Ja                                                            |
| **Indicatie authentiek**         | Authentiek.                                                   |
| **Toelichting attribuut**        | Default: false (geen talud)                                   |

### Associatie: geometrie2dBegroeidTerreindeel

| **Definitie**      | Vlakgeometrie. |
|--------------------|----------------|
| **Doelklasse**     | GM\_Surface    |
| **Multipliciteit** | [1..1]         |
| **Stereotype**     | \<\<BGT\>\>    |
| **Toelichting**    |                |

### Associatie: kruinlijnBegroeidTerreindeel

| **Definitie**      | Lijngeometrie van de hoogstgelegen begrenzing van een kunstmatig aangelegd en onderhouden helling. |
|--------------------|----------------------------------------------------------------------------------------------------|
| **Doelklasse**     | GM\_Curve                                                                                          |
| **Multipliciteit** | [0..1]                                                                                             |
| **Stereotype**     | \<\<BGT\>\> \<\<voidable\>\>                                                                       |
| **Toelichting**    |                                                                                                    |

Waterdeel
---------

### bgt-type

| **Naam attribuut**               | bgt-type                          |
|----------------------------------|-----------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\> |
| **Herkomst attribuut**           | BGT                               |
| **Code attribuut**               | 40.1                              |
| **Definitie attribuut**          | Specificatie van het soort Water. |
| **Waardetype attribuut**         | GenericName                       |
| **Waardenverzameling**           | TypeWater                         |
| **Multipliciteit**               | [1-1]                             |
| **Datum opname**                 |                                   |
| **Indicatie materiële historie** | Nee                               |
| **Indicatie formele historie**   | Ja                                |
| **Indicatie authentiek**         | Authentiek                        |
| **Toelichting attribuut**        |                                   |

### Associatie: geometrie2dWaterdeel

| **Definitie**      | Vlakgeometrie. |
|--------------------|----------------|
| **Doelklasse**     | GM\_Surface    |
| **Multipliciteit** | [1..1]         |
| **Stereotype**     | \<\<BGT\>\>    |
| **Toelichting**    |                |

OndersteunendWaterdeel
----------------------

### bgt-type

| **Naam attribuut**               | bgt-type                          |
|----------------------------------|-----------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\> |
| **Herkomst attribuut**           | BGT                               |
| **Code attribuut**               | 41.1                              |
| **Definitie attribuut**          | Specificatie van het soort Water. |
| **Waardetype attribuut**         | GenericName                       |
| **Waardenverzameling**           | TypeOndersteunendWaterdeel        |
| **Multipliciteit**               | [1-1]                             |
| **Datum opname**                 |                                   |
| **Indicatie materiële historie** | Nee                               |
| **Indicatie formele historie**   | Ja                                |
| **Indicatie authentiek**         | Authentiek                        |
| **Toelichting attribuut**        |                                   |

### Associatie: geometrie2dOndersteunendWaterdeel

| **Definitie**      | Vlakgeometrie. |
|--------------------|----------------|
| **Doelklasse**     | GM\_Surface    |
| **Multipliciteit** | [1..1]         |
| **Stereotype**     | \<\<BGT\>\>    |
| **Toelichting**    |                |

Pand
----

### identificatieBAGPND

| **Naam attribuut**               | identificatieBAGPND                                                                |
|----------------------------------|------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                  |
| **Herkomst attribuut**           | BAG                                                                                |
| **Code attribuut**               | 60.1                                                                               |
| **Definitie attribuut**          | De unieke identificatie van het object zoals is toegekend in de BAG-administratie. |
| **Waardetype attribuut**         | CharacterString                                                                    |
| **Waardenverzameling**           |                                                                                    |
| **Multipliciteit**               | [1-1]                                                                              |
| **Datum opname**                 |                                                                                    |
| **Indicatie materiële historie** | Nee                                                                                |
| **Indicatie formele historie**   | Nee                                                                                |
| **Indicatie authentiek**         | Authentiek andere registratie                                                      |
| **Toelichting attribuut**        |                                                                                    |

### nummeraanduidingreeks

| **Naam attribuut**               | nummeraanduidingreeks                                                                 |
|----------------------------------|---------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                     |
| **Herkomst attribuut**           | BGT                                                                                   |
| **Code attribuut**               | 60.3                                                                                  |
| **Definitie attribuut**          | Bevat de reeks nummeraanduidingen behorend bij het pand ten behoeve van visualisatie. |
| **Waardetype attribuut**         | Nummeraanduidingreeks                                                                 |
| **Waardenverzameling**           |                                                                                       |
| **Multipliciteit**               | [0-\*]                                                                                |
| **Datum opname**                 |                                                                                       |
| **Indicatie materiële historie** | Nee                                                                                   |
| **Indicatie formele historie**   | Ja                                                                                    |
| **Indicatie authentiek**         | Authentiek                                                                            |
| **Toelichting attribuut**        |                                                                                       |

### Associatie: geometrie2dGrondvlak

| **Definitie**      | Vlakgeometrie grondvlak. |
|--------------------|--------------------------|
| **Doelklasse**     | GM\_MultiSurface         |
| **Multipliciteit** | [1..1]                   |
| **Stereotype**     | \<\<BGT\>\>              |
| **Toelichting**    |                          |

OverigeConstructie
------------------

### Associatie: geometrie2dOverigeConstructie

| **Definitie**      | Punt-, lijn-, vlak- of multivlakgeometrie. |
|--------------------|--------------------------------------------|
| **Doelklasse**     | GM\_Object                                 |
| **Multipliciteit** | [1..1]                                     |
| **Stereotype**     | \<\<BGT\>\>                                |
| **Toelichting**    |                                            |

OverigBouwwerk
--------------

### bgt-type

| **Naam attribuut**               | bgt-type                                    |
|----------------------------------|---------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\>                                 |
| **Herkomst attribuut**           | BGT                                         |
| **Code attribuut**               | 53.1                                        |
| **Definitie attribuut**          | Specificatie van het soort overig bouwwerk. |
| **Waardetype attribuut**         | GenericName                                 |
| **Waardenverzameling**           | TypeOverigBouwwerk                          |
| **Multipliciteit**               | [1-1]                                       |
| **Datum opname**                 |                                             |
| **Indicatie materiële historie** | Nee                                         |
| **Indicatie formele historie**   | Ja                                          |
| **Indicatie authentiek**         | Authentiek                                  |
| **Toelichting attribuut**        |                                             |

Overbruggingsdeel
-----------------

### Associatie: geometrie2dOverbruggingsdeel

| **Definitie**      | Vlakgeometrie. |
|--------------------|----------------|
| **Doelklasse**     | GM\_Surface    |
| **Multipliciteit** | [1..1]         |
| **Stereotype**     | \<\<BGT\>\>    |
| **Toelichting**    |                |

Tunneldeel
----------

### Associatie: geometrie2dTunneldeel

| **Definitie**      | Vlakgeometrie. |
|--------------------|----------------|
| **Doelklasse**     | GM\_Surface    |
| **Multipliciteit** | [1..1]         |
| **Stereotype**     | \<\<BGT\>\>    |
| **Toelichting**    |                |

Kunstwerkdeel
-------------

### bgt-type

| **Naam attribuut**               | bgt-type                              |
|----------------------------------|---------------------------------------|
| **Stereotype**                   | \<\<BGT\>\>                           |
| **Herkomst attribuut**           | BGT                                   |
| **Code attribuut**               | 51.1                                  |
| **Definitie attribuut**          | Specificatie van het soort kunstwerk. |
| **Waardetype attribuut**         | GenericName                           |
| **Waardenverzameling**           | TypeKunstwerk                         |
| **Multipliciteit**               | [1-1]                                 |
| **Datum opname**                 |                                       |
| **Indicatie materiële historie** | Nee                                   |
| **Indicatie formele historie**   | Ja                                    |
| **Indicatie authentiek**         | Authentiek                            |
| **Toelichting attribuut**        |                                       |

Scheiding
---------

### bgt-type

| **Naam attribuut**               | bgt-type                              |
|----------------------------------|---------------------------------------|
| **Stereotype**                   | \<\<BGT\>\>                           |
| **Herkomst attribuut**           | BGT                                   |
| **Code attribuut**               | 52.1                                  |
| **Definitie attribuut**          | Specificatie van het soort scheiding. |
| **Waardetype attribuut**         | GenericName                           |
| **Waardenverzameling**           | TypeScheiding                         |
| **Multipliciteit**               | [1-1]                                 |
| **Datum opname**                 |                                       |
| **Indicatie materiële historie** | Nee                                   |
| **Indicatie formele historie**   | Ja                                    |
| **Indicatie authentiek**         | Authentiek                            |
| **Toelichting attribuut**        |                                       |

OngeclassificeerdObject
-----------------------

### Associatie: geometrie2d

| **Definitie**      | Vlakgeometrie. |
|--------------------|----------------|
| **Doelklasse**     | GM\_Surface    |
| **Multipliciteit** | [1..1]         |
| **Stereotype**     | \<\<BGT\>\>    |
| **Toelichting**    |                |

FunctioneelGebied
-----------------

### bgt-type

| **Naam attribuut**               | bgt-type                                       |
|----------------------------------|------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>              |
| **Herkomst attribuut**           | BGT                                            |
| **Code attribuut**               | 350.2                                          |
| **Definitie attribuut**          | Specificatie van het soort Functioneel Gebied. |
| **Waardetype attribuut**         | GenericName                                    |
| **Waardenverzameling**           | TypeFunctioneelGebied                          |
| **Multipliciteit**               | [1-1]                                          |
| **Datum opname**                 |                                                |
| **Indicatie materiële historie** | Nee                                            |
| **Indicatie formele historie**   | Ja                                             |
| **Indicatie authentiek**         | Authentiek.                                    |
| **Toelichting attribuut**        |                                                |

### Associatie: geometrie2dFunctioneelGebied

| **Definitie**      | Vlakgeometrie. |
|--------------------|----------------|
| **Doelklasse**     | GM\_Surface    |
| **Multipliciteit** | [1..1]         |
| **Stereotype**     | \<\<BGT\>\>    |
| **Toelichting**    |                |

OpenbareRuimteLabel
-------------------

### identificatieBAGOPR

| **Naam attribuut**               | identificatieBAGOPR                                                                |
|----------------------------------|------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                  |
| **Herkomst attribuut**           | BAG                                                                                |
| **Code attribuut**               | 11.01                                                                              |
| **Definitie attribuut**          | De unieke identificatie van het object zoals is toegekend in de BAG-administratie. |
| **Waardetype attribuut**         | CharacterString                                                                    |
| **Waardenverzameling**           |                                                                                    |
| **Multipliciteit**               | [1-1]                                                                              |
| **Datum opname**                 |                                                                                    |
| **Indicatie materiële historie** | Nee                                                                                |
| **Indicatie formele historie**   | Nee                                                                                |
| **Indicatie authentiek**         | Authentiek andere registratie                                                      |
| **Toelichting attribuut**        |                                                                                    |

### openbareRuimteNaam

| **Naam attribuut**               | openbareRuimteNaam                                                                                                                                                                                                          |
|----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                                                                                                                                                           |
| **Herkomst attribuut**           | BAG                                                                                                                                                                                                                         |
| **Code attribuut**               | 11.10                                                                                                                                                                                                                       |
| **Definitie attribuut**          | Een door het bevoegde gemeentelijke orgaan aan een OPENBARE RUIMTE toegekende benaming.                                                                                                                                     |
| **Waardetype attribuut**         | Label                                                                                                                                                                                                                       |
| **Waardenverzameling**           |                                                                                                                                                                                                                             |
| **Multipliciteit**               | [1-1]                                                                                                                                                                                                                       |
| **Datum opname**                 |                                                                                                                                                                                                                             |
| **Indicatie materiële historie** | Ja                                                                                                                                                                                                                          |
| **Indicatie formele historie**   | Ja                                                                                                                                                                                                                          |
| **Indicatie authentiek**         | Authentiek andere registratie                                                                                                                                                                                               |
| **Toelichting attribuut**        | Bij dit attribuut is aangegeven dat zowel materiële als formele historie worden bijgehouden. De openbare ruimtenaam is opgenomen in het BGT informatiemodel ten behoeve van visualisatie maar wordt overgenomen uit de BAG. |

### openbareRuimteType

| **Naam attribuut**               | openbareRuimteType                                                                                                                                                                                                          |
|----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                                                                                                                                                           |
| **Herkomst attribuut**           | BAG                                                                                                                                                                                                                         |
| **Code attribuut**               | 11.16                                                                                                                                                                                                                       |
| **Definitie attribuut**          | De aard van de als zodanig benoemde OPENBARE RUIMTE.                                                                                                                                                                        |
| **Waardetype attribuut**         | GenericName                                                                                                                                                                                                                 |
| **Waardenverzameling**           | TypeOpenbareRuimte                                                                                                                                                                                                          |
| **Multipliciteit**               | [1-1]                                                                                                                                                                                                                       |
| **Datum opname**                 |                                                                                                                                                                                                                             |
| **Indicatie materiële historie** | Ja                                                                                                                                                                                                                          |
| **Indicatie formele historie**   | Ja                                                                                                                                                                                                                          |
| **Indicatie authentiek**         | Authentiek andere registratie                                                                                                                                                                                               |
| **Toelichting attribuut**        | Bij dit attribuut is aangegeven dat zowel materiële als formele historie worden bijgehouden. De openbare ruimtenaam is opgenomen in het BGT informatiemodel ten behoeve van visualisatie maar wordt overgenomen uit de BAG. |

Plaatsbepalingspunt
-------------------

### identificatie

| **Naam attribuut**               | identificatie                                                                              |
|----------------------------------|--------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                          |
| **Herkomst attribuut**           | BGT                                                                                        |
| **Code attribuut**               | 120.1                                                                                      |
| **Definitie attribuut**          | Uniek identificatienummer voor het object dat onveranderlijk is zolang het object bestaat. |
| **Waardetype attribuut**         | NEN3610ID                                                                                  |
| **Waardenverzameling**           |                                                                                            |
| **Multipliciteit**               | [1-1]                                                                                      |
| **Datum opname**                 |                                                                                            |
| **Indicatie materiële historie** | Nee                                                                                        |
| **Indicatie formele historie**   | Nee                                                                                        |
| **Indicatie authentiek**         | Authentiek                                                                                 |
| **Toelichting attribuut**        | Zie 3.10 van de gegevenscatalogus.                                                         |

### nauwkeurigheid

| **Naam attribuut**               | nauwkeurigheid                                                                                                                          |
|----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\> \<\<voidable\>\>                                                                                      |
| **Herkomst attribuut**           | BGT                                                                                                                                     |
| **Code attribuut**               | 120.2                                                                                                                                   |
| **Definitie attribuut**          | Gerealiseerde geometrische nauwkeurigheid van de geometrie van het object ten opzichte van de werkelijkheid, uitgedrukt in centimeters. |
| **Waardetype attribuut**         | Integer                                                                                                                                 |
| **Waardenverzameling**           |                                                                                                                                         |
| **Multipliciteit**               | [1-1]                                                                                                                                   |
| **Datum opname**                 |                                                                                                                                         |
| **Indicatie materiële historie** | Nee                                                                                                                                     |
| **Indicatie formele historie**   | Nee                                                                                                                                     |
| **Indicatie authentiek**         | Authentiek                                                                                                                              |
| **Toelichting attribuut**        |                                                                                                                                         |

### datumInwinning

| **Naam attribuut**               | datumInwinning                                                                                                                                       |
|----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                                                                                    |
| **Herkomst attribuut**           | BGT                                                                                                                                                  |
| **Code attribuut**               | 120.3                                                                                                                                                |
| **Definitie attribuut**          | Datum waarop het punt is ingewonnen.                                                                                                                 |
| **Waardetype attribuut**         | Date                                                                                                                                                 |
| **Waardenverzameling**           |                                                                                                                                                      |
| **Multipliciteit**               | [1-1]                                                                                                                                                |
| **Datum opname**                 |                                                                                                                                                      |
| **Indicatie materiële historie** | Nee                                                                                                                                                  |
| **Indicatie formele historie**   | Nee                                                                                                                                                  |
| **Indicatie authentiek**         | Authentiek                                                                                                                                           |
| **Toelichting attribuut**        | Als de inwinningsdatum van het punt tijdens transitie onbekend is, moet hier de datum van de transitie (gelijk aan objectBeginTijd) worden ingevuld. |

### inwinnendeInstantie

| **Naam attribuut**               | inwinnendeInstantie                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
|----------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\> \<\<voidable\>\>                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Herkomst attribuut**           | BGT                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Code attribuut**               | 120.4                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Definitie attribuut**          | De organisatie die namens de bronhouder het object inwint.                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Waardetype attribuut**         | CharacterString                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Waardenverzameling**           |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Multipliciteit**               | [1-1]                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Datum opname**                 |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Indicatie materiële historie** | Nee                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Indicatie formele historie**   | Nee                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Indicatie authentiek**         | Authentiek                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Toelichting attribuut**        | De inwinnende instantie kan de bronhouder zelf zijn of een organisatie aan wie dit is gedelegeerd. De Codelist is dezelfde lijst als die van de bronhouder van het BGTObject, maar dan uitgebreid met de inwinnende instanties. Indien de inwinnende instantie voor haar uitvoerende taak gebruik maakt van externe organisaties (zoals landmeetkundige bureaus) dan worden deze laatsten NIET aan de CodeList toegevoegd maar vullen zij de inwinnende instantie in voor wie zij het werk uitvoeren. |

### inwinningsmethode

| **Naam attribuut**               | inwinningsmethode                       |
|----------------------------------|-----------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>       |
| **Herkomst attribuut**           | BGT                                     |
| **Code attribuut**               | 120.5                                   |
| **Definitie attribuut**          | De wijze waarop het punt is ingewonnen. |
| **Waardetype attribuut**         | GenericName                             |
| **Waardenverzameling**           | Inwinningsmethode                       |
| **Multipliciteit**               | [1-1]                                   |
| **Datum opname**                 |                                         |
| **Indicatie materiële historie** | Nee                                     |
| **Indicatie formele historie**   | Nee                                     |
| **Indicatie authentiek**         | Authentiek                              |
| **Toelichting attribuut**        |                                         |

### Associatie: geometrie

| **Definitie**      | Puntgeometrie. |
|--------------------|----------------|
| **Doelklasse**     | GM\_Point      |
| **Multipliciteit** | [1..1]         |
| **Stereotype**     | \<\<BGT\>\>    |
| **Toelichting**    |                |

Nummeraanduidingreeks
---------------------

### nummeraanduidingreeks

| **Naam attribuut**               | nummeraanduidingreeks                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Herkomst attribuut**           | BGT                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Code attribuut**               | 60.3.1                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Definitie attribuut**          | Bevat de reeks nummeraanduidingen behorend bij het pand ten behoeve van visualisatie.                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Waardetype attribuut**         | Label                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Waardenverzameling**           |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Multipliciteit**               | [1-1]                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Datum opname**                 |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Indicatie materiële historie** | Nee                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Indicatie formele historie**   | Ja                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Indicatie authentiek**         | Authentiek                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Toelichting attribuut**        | Om een reeks nummeraanduidingen op te nemen ten behoeve van visualisatie. Dit wordt geautomatiseerd afgeleid uit de BAG, waarbij het laagste en hoogste huisnummer van nummeraanduidingen van verblijfsobjecten in een pand worden weergegeven. - Voor hoekpanden waarbij verblijfsobjecten uit verschillende openbare ruimten zijn opgenomen, is het mogelijk om meerdere nummeraanduidingreeksen op te nemen. - Meerdere huisnummers in een pand worden niet individueel afgebeeld, laat staan de bijbehorende huisletters en toevoegingen. |

### identificatieBAGVBOLaagsteHuisnummer

| **Naam attribuut**               | identificatieBAGVBOLaagsteHuisnummer                                                                           |
|----------------------------------|----------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                                              |
| **Herkomst attribuut**           | BGT                                                                                                            |
| **Code attribuut**               | 60.3.2                                                                                                         |
| **Definitie attribuut**          | Identificatie in de BAG registratie van het verblijfsobject met het laagste huisnummer behorende tot de reeks. |
| **Waardetype attribuut**         | CharacterString                                                                                                |
| **Waardenverzameling**           |                                                                                                                |
| **Multipliciteit**               | [1-1]                                                                                                          |
| **Datum opname**                 |                                                                                                                |
| **Indicatie materiële historie** | Nee                                                                                                            |
| **Indicatie formele historie**   | Ja                                                                                                             |
| **Indicatie authentiek**         | Authentiek andere registratie                                                                                  |
| **Toelichting attribuut**        |                                                                                                                |

### identificatieBAGVBOHoogsteHuisnummer

| **Naam attribuut**               | identificatieBAGVBOHoogsteHuisnummer                                                                           |
|----------------------------------|----------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                                              |
| **Herkomst attribuut**           | BGT                                                                                                            |
| **Code attribuut**               | 60.3.3                                                                                                         |
| **Definitie attribuut**          | Identificatie in de BAG registratie van het verblijfsobject met het hoogste huisnummer behorende tot de reeks. |
| **Waardetype attribuut**         | CharacterString                                                                                                |
| **Waardenverzameling**           |                                                                                                                |
| **Multipliciteit**               | [0-1]                                                                                                          |
| **Datum opname**                 |                                                                                                                |
| **Indicatie materiële historie** | Nee                                                                                                            |
| **Indicatie formele historie**   | Ja                                                                                                             |
| **Indicatie authentiek**         | Authentiek andere registratie                                                                                  |
| **Toelichting attribuut**        |                                                                                                                |

NEN3610ID
---------

### namespace

| **Naam attribuut**               | namespace                                                                                                                                                                                                                                                                                                                                                                |
|----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                                                                                                                                                                                                                                                                                                        |
| **Herkomst attribuut**           | BGT                                                                                                                                                                                                                                                                                                                                                                      |
| **Code attribuut**               | 10.1.1                                                                                                                                                                                                                                                                                                                                                                   |
| **Definitie attribuut**          | Unieke verwijzing naar een registratie van objecten.                                                                                                                                                                                                                                                                                                                     |
| **Waardetype attribuut**         | CharacterString                                                                                                                                                                                                                                                                                                                                                          |
| **Waardenverzameling**           |                                                                                                                                                                                                                                                                                                                                                                          |
| **Multipliciteit**               | [1-1]                                                                                                                                                                                                                                                                                                                                                                    |
| **Datum opname**                 |                                                                                                                                                                                                                                                                                                                                                                          |
| **Indicatie materiële historie** | Nee                                                                                                                                                                                                                                                                                                                                                                      |
| **Indicatie formele historie**   | Nee                                                                                                                                                                                                                                                                                                                                                                      |
| **Indicatie authentiek**         | Authentiek                                                                                                                                                                                                                                                                                                                                                               |
| **Toelichting attribuut**        | Het attribuut ‘namespace’ is een unieke verwijzing naar de registratie die de identificatie uitdeelt. Deze lijst van registraties wordt beheerd door de beheerder van NEN3610. Binnen Nederland zal deze namespace vrijwel altijd met ‘NL.’ beginnen. De volgende karakters mogen in een namespace aanduiding voorkomen: {”A” …”Z”, “a”…”z”,”0”…”9”, “\_”, “-“, “,”,”.”} |

### lokaalID

| **Naam attribuut**               | lokaalID                                                                                                                                                                                                                                               |
|----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                                                                                                                                                                                      |
| **Herkomst attribuut**           | BGT                                                                                                                                                                                                                                                    |
| **Code attribuut**               | 10.1.2                                                                                                                                                                                                                                                 |
| **Definitie attribuut**          | Unieke identificatiecode binnen een registratie.                                                                                                                                                                                                       |
| **Waardetype attribuut**         | CharacterString                                                                                                                                                                                                                                        |
| **Waardenverzameling**           |                                                                                                                                                                                                                                                        |
| **Multipliciteit**               | [1-1]                                                                                                                                                                                                                                                  |
| **Datum opname**                 |                                                                                                                                                                                                                                                        |
| **Indicatie materiële historie** | Nee                                                                                                                                                                                                                                                    |
| **Indicatie formele historie**   | Nee                                                                                                                                                                                                                                                    |
| **Indicatie authentiek**         | Authentiek                                                                                                                                                                                                                                             |
| **Toelichting attribuut**        | LokaalID is de identificatiecode die een object heeft binnen een (lokaal) registratie. De volgende karakters mogen in een lokaalID voorkomen: {”A” …”Z”, “a”…”z”,”0”…”9”, “\_”, “-“, “,”,”.”} Dit is de IMGeo identificatie. Een betekenisloos nummer. |

Label
-----

### tekst

| **Naam attribuut**               | tekst                             |
|----------------------------------|-----------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\> |
| **Herkomst attribuut**           | BGT                               |
| **Code attribuut**               | 11.10.1                           |
| **Definitie attribuut**          | Tekst voor het label.             |
| **Waardetype attribuut**         | CharacterString                   |
| **Waardenverzameling**           |                                   |
| **Multipliciteit**               | [1-1]                             |
| **Datum opname**                 |                                   |
| **Indicatie materiële historie** | Nee                               |
| **Indicatie formele historie**   | zie groep                         |
| **Indicatie authentiek**         |                                   |
| **Toelichting attribuut**        |                                   |

### positie

| **Naam attribuut**               | positie                                                       |
|----------------------------------|---------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                             |
| **Herkomst attribuut**           | BGT                                                           |
| **Code attribuut**               | 11.10.2                                                       |
| **Definitie attribuut**          | Labelpositie, samengesteld uit plaatsingspunt en rotatiehoek. |
| **Waardetype attribuut**         | Labelpositie                                                  |
| **Waardenverzameling**           |                                                               |
| **Multipliciteit**               | [1-\*]                                                        |
| **Datum opname**                 |                                                               |
| **Indicatie materiële historie** | Nee                                                           |
| **Indicatie formele historie**   | Nee                                                           |
| **Indicatie authentiek**         | Zie groep                                                     |
| **Toelichting attribuut**        |                                                               |

Labelpositie
------------

### plaatsingspunt

| **Naam attribuut**               | plaatsingspunt                                                  |
|----------------------------------|-----------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                               |
| **Herkomst attribuut**           | BGT                                                             |
| **Code attribuut**               | 11.10.2.1                                                       |
| **Definitie attribuut**          | Coördinaten voor de locatie waar het label moet worden getoond. |
| **Waardetype attribuut**         | GM\_Point                                                       |
| **Waardenverzameling**           |                                                                 |
| **Multipliciteit**               | [1-1]                                                           |
| **Datum opname**                 |                                                                 |
| **Indicatie materiële historie** | Nee                                                             |
| **Indicatie formele historie**   | Nee                                                             |
| **Indicatie authentiek**         | Authentiek                                                      |
| **Toelichting attribuut**        |                                                                 |

### hoek

| **Naam attribuut**               | hoek                                                                                                  |
|----------------------------------|-------------------------------------------------------------------------------------------------------|
| **Stereotype**                   | \<\<BGT\>\> \<\<attribuuttype\>\>                                                                     |
| **Herkomst attribuut**           | BGT                                                                                                   |
| **Code attribuut**               | 11.10.2.2                                                                                             |
| **Definitie attribuut**          | De rotatie van het label bij visualisatie, met de klok mee ten opzichte van de normale tekstrichting. |
| **Waardetype attribuut**         | Real                                                                                                  |
| **Waardenverzameling**           |                                                                                                       |
| **Multipliciteit**               | [1-1]                                                                                                 |
| **Datum opname**                 |                                                                                                       |
| **Indicatie materiële historie** | Nee                                                                                                   |
| **Indicatie formele historie**   | Nee                                                                                                   |
| **Indicatie authentiek**         | Authentiek                                                                                            |
| **Toelichting attribuut**        |                                                                                                       |

# Domeinwaarden

Hieronder volgt een specificatie van de domeinwaarden en hun definities voor de relevante attributen. De domeinwaarden bij een attribuut hebben een vaste volgorde. Deze volgorde geeft waar nodig een hiërarchie aan, die van belang is bij elkaar kruisende objecten, waarbij de eerstgenoemde domeinwaarde de belangrijkste is.

## Status

| bestaand | Situatie waarin het object wordt / kan worden gebruikt voor het doel waarvoor het is gebouwd / aangelegd. (bron: IMGEO 1.0) |
|----------|-----------------------------------------------------------------------------------------------------------------------------|


FunctieWeg
----------

| OV-baan                | Wegdeel dat uitsluitend is bestemd en gemarkeerd voor openbaar vervoer en afgescheiden is van de andere wegdelen niet uitsluitend door markering. (bron: BGT)                                                    |
|------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| overweg                | Een gelijkvloerse kruising van een wegdeel en een wegdeel type ov-baan met spoor type trein of sneltram. (bron: BGT)                                                                                             |
| spoorbaan              | Gebaand gedeelte voor het verkeer over rails. (bron: NEN 3610)                                                                                                                                                   |
| baan voor vliegverkeer | Wegdeel uitsluitend bedoeld voor vliegverkeer. (bron: BGT)                                                                                                                                                       |
| rijbaan autosnelweg    | Wegdeel dat onderdeel is van een weg uitsluitend bestemd voor snelverkeer en met gescheiden rijbanen en ongelijkvloerse kruisingen, daartoe aangeduid met het betreffende verkeersbord. (bron: BGT)              |
| rijbaan autoweg        | Wegdeel dat onderdeel is van een weg uitsluitend bestemd voor snelverkeer, daartoe aangeduid met het betreffende verkeersbord. (bron: BGT)                                                                       |
| rijbaan regionale weg  | Wegdeel dat onderdeel is van een weg die een verbinding vormt tussen bewoonde oorden of tussen wijken binnen een dorp of stad. (bron: BGT)                                                                       |
| rijbaan lokale weg     | Wegdeel dat onderdeel is van een weg van lokaal belang. (bron: BGT)                                                                                                                                              |
| fietspad               | Wegdeel met name bestemd voor fietsers en, indien toegestaan, bromfietsers en dat afgescheiden is van de andere wegdelen niet uitsluitend door markering. (bron: BGT)                                            |
| voetpad                | Wegdeel waar voetgangers gebruik van moeten maken. (bron: BGT)                                                                                                                                                   |
| voetpad op trap        | Voetpad op verkeersinfrastructurele voorziening bestaande uit een constructie van treden, waarop men een hoger of lager gelegen plaats kan bereiken. (bron: BGT)                                                 |
| ruiterpad              | Een wegdeel primair aangelegd voor het gebruik door ruiters. (bron: BGT)                                                                                                                                         |
| parkeervlak            | Wegdeel bestemd voor het parkeren van motorvoertuigen. (bron: IMGEO 1.0)                                                                                                                                         |
| voetgangersgebied      | Wegdeel alleen voor het gebruik door voetgangers, waarbij het door voetgangers te gebruiken gebied de volle breedte van de weg beslaat en het gebied een nadrukkelijk openbaar karakter heeft. (bron: IMGEO 1.0) |
| inrit                  | Toegangswegen, oprijlanen en dergelijke met verkeersfunctie die leiden naar afgelegen erven en terreinen. (bron: IMGEO 2.0)                                                                                      |
| woonerf                | Wegdeel waar de verblijfsfunctie (lopen, spelen, ontmoeten enzovoorts) prioriteit heeft boven de verkeersfunctie. (bron: IMGEO 1.0)                                                                              |
| transitie              | De waarde is tijdens transitie niet bekend. (bron: BGT)                                                                                                                                                          |

FysiekVoorkomenWeg
------------------

| gesloten verharding | Verharding bestaande uit een materiaal dat niet verwijderbaar is zonder definitieve destructie, zoals bijvoorbeeld bitumen, cement of kunststof. (bron: IMGEO 1.0) |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| open verharding     | Verharding gevormd door in verband aangebrachte elementen van beperkte afmetingen, zoals bijvoorbeeld klinkers en tegels. (bron: IMGEO 1.0)                        |
| half verhard        | Verharding bestaande uit een door verdichting gebonden materiaal, of onsamenhangend materiaal. (bron: BGT)                                                         |
| onverhard           | Wegdelen waar geen verharding of aaneengesloten vegetatie aanwezig is. (bron: IMGEO 1.0)                                                                           |
| transitie           | De waarde is tijdens transitie niet bekend. (bron: BGT)                                                                                                            |

FunctieOndersteunendWegdeel
---------------------------

| verkeerseiland | Ondersteunend wegdeel van beperkte omvang, uitgevoerd als verhoging of wegmarkering, dat wordt omsloten door wegdelen en ten doel heeft verkeersstromen te scheiden. (bron: CROW) |
|----------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| berm           | Een strook grond langs een weg of spoorweg. (bron: BGT)                                                                                                                           |
| transitie      | De waarde is tijdens transitie niet bekend. (bron: BGT)                                                                                                                           |

FysiekVoorkomenOndersteunendWegdeel
-----------------------------------

| gesloten verharding | Verharding bestaande uit een materiaal dat niet verwijderbaar is zonder definitieve destructie, zoals bijvoorbeeld bitumen, cement of kunststof. (bron: BGT) |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| open verharding     | Verharding gevormd door in verband aangebrachte elementen van beperkte afmetingen, zoals bijvoorbeeld klinkers en tegels. (bron: BGT)                        |
| half verhard        | Verharding bestaande uit een door verdichting gebonden materiaal, of onsamenhangend materiaal. (bron: BGT)                                                   |
| onverhard           | Wegdelen waar geen verharding of aaneengesloten vegetatie aanwezig is. (bron: BGT)                                                                           |
| groenvoorziening    | Terreindeel met aangelegde beplanting, meestal gras, heesters of struiken. (bron: BGT)                                                                       |
| transitie           | De waarde is tijdens transitie niet bekend. (bron: BGT)                                                                                                      |

FunctieSpoor
------------

| trein     | Spoor voor een railvoertuig voor de langere afstand dat sneller dan 45 km per uur kan, bestaande uit een enkele of een reeks van locomotieven, treinstellen en/of wagons. (bron: BGT) |
|-----------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| sneltram  | Spoor voor een boven- danwel ondergrondse interlokale tram met een vrije baan. (bron: BGT)                                                                                            |
| tram      | Spoor voor een railvoertuig voor personenvervoer voor de korte afstand. (bron: BGT)                                                                                                   |
| transitie | De waarde is tijdens transitie niet bekend. (bron: BGT)                                                                                                                               |
| niet-bgt  | Het object is geen BGT object. (bron: BGT 1.1)                                                                                                                                        |

FysiekVoorkomenOnbegroeidTerrein
--------------------------------

| erf                 | Terreindeel dat bij een pand of overig bouwwerk hoort, dat niet nader wordt ingewonnen en dat bestaat uit een mengvorm van begroeiing, verharding, en/of water. (bron: IMGEO 1.0) |
|---------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| gesloten verharding | Verharding bestaande uit een materiaal dat niet verwijderbaar is zonder definitieve destructie, zoals bijvoorbeeld bitumen, cement of kunststof. (bron: IMGEO 1.0)                |
| open verharding     | Verharding gevormd door in verband aangebrachte elementen van beperkte afmetingen, zoals bijvoorbeeld klinkers en tegels. (bron: IMGEO 1.0)                                       |
| half verhard        | Verharding bestaande uit een door verdichting gebonden materiaal, of onsamenhangend materiaal. (bron: BGT)                                                                        |
| onverhard           | Terreindeel waar geen verharding of aaneengesloten vegetatie aanwezig is, niet zijnde zand. Braakliggend valt hier wel onder. (bron: IMGEO 1.0)                                   |
| zand                | Terreindeel dat grotendeels bedekt is met zand. (bron: BGT)                                                                                                                       |
| transitie           | De waarde is tijdens transitie niet bekend. (bron: BGT)                                                                                                                           |

FysiekVoorkomenBegroeidTerrein
------------------------------

| loofbos            | Terreindeel begroeid met een dusdanige aantal loofbomen dat deze een min of meer gesloten geheel vormen of, na volgroeiing van de bomen, zullen vormen. (bron: BGT)                                                                   |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| gemengd bos        | Terreindeel begroeid met een dusdanige aantal naald- en loofbomen dat deze een min of meer gesloten geheel vormen of, na volgroeiing van de bomen, zullen vormen. (bron: BGT)                                                         |
| naaldbos           | Terreindeel begroeid met een dusdanige aantal naaldbomen dat deze een min of meer gesloten geheel vormen of, na volgroeiing van de bomen, zullen vormen. (bron: BGT)                                                                  |
| heide              | Terreindeel overwegend begroeid met heide en heideachtige vegetaties. (bron: BGT)                                                                                                                                                     |
| struiken           | Terreindeel bedekt met niet-gecultiveerde (natuurlijke), lage, houtachtige, overblijvende planten gekenmerkt door verschillende vertakkingen dicht bij de wortel en afwezigheid van opvallende stammen. (bron: BGT)                   |
| houtwal            | Terreindeel zijnde een afscheiding met beperkte breedte en beplant met bomen of struiken. (bron: BGT)                                                                                                                                 |
| duin               | Verhoging of heuvel van zand of fijne losse aarde en verpulverd gesteente opgeworpen door wind of door stromend water. (bron: )                                                                                                       |
| grasland overig    | Terreindeel met een vegetatie bestaande uit grassen en of grasachtigen, en met de in graslanden voorkomende kruiden, dat niet in gebruik is voor agrarische doeleinden. (bron: BGT)                                                   |
| moeras             | Terreindeel met moerasvegetatie in stilstaand water van geringe diepte zonder merkbare toe- of afvloeiing. (bron: BGT)                                                                                                                |
| rietland           | Terreindeel overwegend begroeid met rietvegetatie. (bron: BGT)                                                                                                                                                                        |
| kwelder            | Buitendijks gelegen aangeslibd land van een wad, dat bij gewone vloed niet meer onder loopt. (bron: aquo)                                                                                                                             |
| fruitteelt         | Terreindeel begroeid met fruitbomen in de vorm van hoogstam en laagstamboomgaard, druiven of kleinfruit. (bron: BGT)                                                                                                                  |
| boomteelt          | Grond in gebruik voor het kweken van jonge siergewassen, bomen enz. ten behoeve van een later gebruik elders. (bron: CROW)                                                                                                            |
| bouwland           | Terreindeel in gebruik als akker, met gewassen die in een teelt roulatieschema zijn opgenomen. Kan tijdelijk zonder gewas zijn of braak liggen. (bron: BGT)                                                                           |
| grasland agrarisch | Terreindeel met een vegetatie bestaande uit grassen en of grasachtigen, en met de in graslanden voorkomende kruiden, zijnde cultuurgrasland dat in gebruik is voor de veeteelt, bijvoorbeeld als weiland of als hooiland. (bron: BGT) |
| groenvoorziening   | Terreindeel met aangelegde beplanting, meestal gras, heesters of struiken. (bron: BGT)                                                                                                                                                |
| transitie          | De waarde is tijdens transitie niet bekend. (bron: BGT)                                                                                                                                                                               |

TypeWater
---------

| zee                  | Uitgestrekt oppervlak zout water. (bron: IMGEO 1.0)                                                                                  |
|----------------------|--------------------------------------------------------------------------------------------------------------------------------------|
| waterloop            | Een voor de waterbeheersing bestemde geul die meestal permanent water bevat (zoals rivier, kanaal, beek, sloot, gracht). (bron: BGT) |
| watervlakte          | Alle oppervlakken die vrij permanent met zoet water zijn bedekt. (zoals meer, plas, ven, vijver). (bron: IMGEO 1.0)                  |
| greppel, droge sloot | Een ten behoeve van de waterbeheersing gegraven geul die al dan niet met water bedekt is. (bron: IMGEO 1.0)                          |
| transitie            | De waarde is tijdens transitie niet bekend. (bron: BGT)                                                                              |

TypeOndersteunendWaterdeel
--------------------------

| oever, slootkant | De strook land die in direct contact staat met water, inclusief het gebied tussen de hoogwaterlijn en laagwaterlijn. (bron: Inspire) |
|------------------|--------------------------------------------------------------------------------------------------------------------------------------|
| slik             | Buitendijks aangeslibde, onbegroeide grond die bij vrijwel elk hoogwater onderloopt. (bron: aquo)                                    |
| transitie        | De waarde is tijdens transitie niet bekend. (bron: BGT)                                                                              |

TypeOverigBouwwerk
------------------

| overkapping | Een afzonderlijk staande overdekking rustend op kolommen. (bron: BGT)                                                                             |
|-------------|---------------------------------------------------------------------------------------------------------------------------------------------------|
| open loods  | Niet verplaatsbaar licht gebouw met een open gevel, bestemd als berg- of werkplaats of als tijdelijk onderdak voor andere doeleinden. (bron: BGT) |
| opslagtank  | Opslagfaciliteit voor vloeistoffen. Alleen bovengrondse opslagtanks worden opgenomen. (bron: BGT)                                                 |
| bezinkbak   | Een gesloten reservoir waarin het afvalwater tijdelijk wordt opgevangen met een slibreinigende voorziening. (bron: BGT)                           |
| windturbine | Turbine waarin winddruk omgezet wordt in mechanische energie. (bron: BGT)                                                                         |
| lage trafo  | Bouwwerk waarin transformator(en) zijn geplaatst voor elektriciteitsvoorziening. (bron: BGT)                                                      |
| bassin      | Waterbak, zoals een zwembad of een dok. (bron: BGT)                                                                                               |
| transitie   | De waarde is tijdens transitie niet bekend. (bron: BGT)                                                                                           |
| niet-bgt    | Het object is geen BGT object. (bron: BGT 1.1)                                                                                                    |

TypeKunstwerk
-------------

| hoogspanningsmast | Metalen mast of stellage ter ondersteuning van geleidedraden voor het transport van elektriciteit met een hoog voltage. (bron: IMGEO 1.0)                             |
|-------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| gemaal            | Een kunstwerk in principe bedoeld om water van een laag peil naar een hoog peil te brengen. (bron: BGT)                                                               |
| perron            | Verhoogde constructie langs een spoorrail of tramrail voor het in- en uitstappen van passagiers of voor het laden en lossen van goederen. (bron: BGT)                 |
| sluis             | Een kunstmatige, beweegbare waterkering die de verbinding tussen twee wateren kan afsluiten of openstellen en daartoe van deuren of schuiven is voorzien. (bron: BGT) |
| strekdam          | Constructie in het water ter verdediging van de kust/oever. (bron: IMGEO 1.0)                                                                                         |
| steiger           | Vaste (niet drijvende) waterbouwkundige constructie voor het aanleggen van schepen en bedoeld om deze schepen vanaf de wal te laden en te lossen. (bron: IMGEO 1.0)   |
| stuw              | Een constructie met een vaste drempel of een beweegbare klep, die dient om de waterstand boven- en benedenstrooms te regelen. (bron: BGT)                             |
| transitie         | De waarde is tijdens transitie niet bekend. (bron: BGT)                                                                                                               |
| niet-bgt          | Het object is geen BGT object. (bron: BGT 1.1)                                                                                                                        |

TypeScheiding
-------------

| muur           | Een scheiding gemaakt van steen. (bron: BGT)                                                                                      |
|----------------|-----------------------------------------------------------------------------------------------------------------------------------|
| kademuur       | Verticale wand ter scheiding van land en water, opgebouwd uit een muur van gemetselde stenen of gestort beton. (bron: BGT)        |
| geluidsscherm  | Een scheiding bedoeld om geluidshinder in de buitenlucht te verminderen. (bron: BGT)                                              |
| damwand        | Een grondkerende constructie die bestaat uit een verticaal in de grond geplaatste wand. (bron: BGT)                               |
| walbescherming | Een nagenoeg verticale wand tot kering van grond om afkalving van water te voorkomen, niet zijnde een kademuur. (bron: IMGEO 1.0) |
| hek            | Een hekwerk of schutting, typisch ten behoeve van erfafscheiding. (bron: BGT)                                                     |
| transitie      | De waarde is tijdens transitie niet bekend. (bron: BGT)                                                                           |
| niet-bgt       | Het object is geen BGT object. (bron: BGT 1.1)                                                                                    |

TypeOpenbareRuimte
------------------

| Weg                    | Gebaand gedeelte voor het wegverkeer en vliegverkeer te land. (bron: NEN 3610:2011)                                                                                                                                                                               |
|------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Water                  | Grondoppervlak in principe bedekt met water. (bron: NEN 3610:2011)                                                                                                                                                                                                |
| Spoorbaan              | Gebaand gedeelte voor het verkeer over rails. (bron: NEN 3610:2011)                                                                                                                                                                                               |
| Terrein                | Door een fysiek voorkomen gekarakteriseerd zichtbaar begrensd stuk grond. (bron: NEN 3610:2011)                                                                                                                                                                   |
| Kunstwerk              | Civiel-technisch werk voor de infrastructuur van wegen, water, spoorbanen, waterkeringen en/of leidingen en niet bedoeld voor permanent menselijk verblijf. (bron: NEN 3610:2011)                                                                                 |
| Landschappelijk gebied | Definitie ontbreekt in de BAG. (bron: -)                                                                                                                                                                                                                          |
| Administratief gebied  | Een niet tastbaar begrensd grondoppervlak dat als eenheid geldt voor bestuurlijke verantwoordelijkheid, voor bedrijfsvoering, waarbinnen een specifieke rechtsverhouding te onderscheiden is of waarvoor een specifieke functie of bestemming geldt. (bron: aquo) |

TypeFunctioneelGebied
---------------------

| kering   | Een waterkerende en / of scheidende, kunstmatige of natuurlijke hoogte of hooggelegen gronden inclusief de daarin aanwezige waterkerende elementen. (bron: aquo) |
|----------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| niet-bgt | Het object is geen BGT object. (bron: BGT 1.1)                                                                                                                   |

Inwinningsmethode
-----------------

| terrestrisch     | De geometrie is ingewonnen middels terreinbezoek. (bron: BGT)                                          |
|------------------|--------------------------------------------------------------------------------------------------------|
| laser            | De geometrie is met behulp van een laserscanner ingewonnen. (bron: BGT)                                |
| fotogrammetrisch | De geometrie is ingewonnen vanaf daartoe geschikte (digitale) foto's, meestal luchtfoto's. (bron: BGT) |
| panoramabeelden  | De geometrie is vanaf panoramafoto's ingewonnen. (bron: BGT)                                           |
| digitaliseren    | De geometrie is handmatig van analoog naar digitale informatie omgezet. (bron: BGT)                    |
| scannen          | De geometrie is geautomatiseerd van analoog naar digitale informatie omgezet. (bron: BGT)              |
| bouwtekening     | De geometrie is van een bouwtekening afgeleid. (bron: BGT)                                             |
| geconstrueerd    | De geometrie is in een GIS of CAD systeem geconstrueerd. (bron: BGT)                                   |
| transitie        | De gebruikte inwinningsmethode is tijdens transitie niet bekend. (bron: BGT)                           |

VoidReasonValue
---------------

| geenWaarde          | Element heeft in werkelijkheid geen waarde. (bron: NEN 3610:2011)                                                                                                                                                                                      |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| nietOndersteund     | Zender houdt in zijn registratie geen waarde voor dit attribuut bij. Geldt voor alle objecten van dit objecttype. (bron: NEN 3610:2011)                                                                                                                |
| waardeOnbekend      | Element is verplicht maar de waarde is bij de zender niet bekend. (bron: NEN 3610:2011)                                                                                                                                                                |
| vastgesteldOnbekend | Er is vastgesteld dat de waarde van het attribuut onbekend is en hoogst waarschijnlijk niet meer kan worden achterhaald (bijvoorbeeld omdat het brondocument onleesbaar is of het object niet meer bestaat in de werkelijkheid). (bron: NEN 3610:2011) |
| nietGeautoriseerd   | Deze zender vindt dat de ontvanger niet geautoriseerd is om de waarde te kennen. (bron: NEN 3610:2011)                                                                                                                                                 |
