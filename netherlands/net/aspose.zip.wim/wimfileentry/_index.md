---
title: Class WimFileEntry
second_title: Aspose.ZIP voor .NET API-referentie
description: Aspose.Zip.Wim.WimFileEntry klas. Vertegenwoordigt een enkel bestand binnen het wimarchief.
type: docs
weight: 790
url: /nl/net/aspose.zip.wim/wimfileentry/
---
## WimFileEntry class

Vertegenwoordigt een enkel bestand binnen het wim-archief.

```csharp
public sealed class WimFileEntry : WimEntry, IArchiveFileEntry
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [AlternateDataStreams](../../aspose.zip.wim/wimentry/alternatedatastreams/) { get; } | Haalt de namen op van de alternatieve gegevensstromen voor een bestand of directory. |
| [Archive](../../aspose.zip.wim/wimentry/archive/) { get; } | Haalt het archief op waartoe het item behoort. |
| [ChangeTime](../../aspose.zip.wim/wimentry/changetime/) { get; } | Krijgt de laatste keer dat het bestand of de map is gewijzigd. |
| [CreationTime](../../aspose.zip.wim/wimentry/creationtime/) { get; } | Krijgt de aanmaaktijd van het bestand of de map. |
| [FileAttributes](../../aspose.zip.wim/wimentry/fileattributes/) { get; } | Haalt de bestands- of mapkenmerken op. |
| [FullPath](../../aspose.zip.wim/wimentry/fullpath/) { get; } | Krijgt het volledige pad van het item binnen de afbeelding. |
| [HardLink](../../aspose.zip.wim/wimentry/hardlink/) { get; } | Haalt de hardlink-id van het bestand of de map op. |
| [HasHardLinks](../../aspose.zip.wim/wimentry/hashardlinks/) { get; } | Krijgt of het bestand of de map bekend is onder andere namen. |
| [Image](../../aspose.zip.wim/wimentry/image/) { get; } | Haalt de afbeelding op waar het item bij hoort. |
| [IsDirectory](../../aspose.zip.wim/wimentry/isdirectory/) { get; } | Krijgt een waarde die aangeeft of de vermelding een directory vertegenwoordigt. |
| [LastAccessTime](../../aspose.zip.wim/wimentry/lastaccesstime/) { get; } | Haalt de laatste toegangstijd van het bestand of de map op. |
| [LastWriteTime](../../aspose.zip.wim/wimentry/lastwritetime/) { get; } | Krijgt de wijzigingstijd van het bestand of de map. |
| [Length](../../aspose.zip.wim/wimfileentry/length/) { get; } | Krijgt de lengte van het item in bytes. |
| [Name](../../aspose.zip.wim/wimentry/name/) { get; } | Krijgt de naam van het item binnen de afbeelding. |
| [Parent](../../aspose.zip.wim/wimentry/parent/) { get; } | Haalt de bovenliggende map op waartoe het item behoort. |
| [ShortName](../../aspose.zip.wim/wimentry/shortname/) { get; } | Krijgt korte naam van het item binnen afbeelding. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract_1)(Stream) | Extraheert de ingang van de geleverde stream. |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract)(string) | Extraheert de invoer naar het bestandssysteem via het opgegeven pad. |
| [Open](../../aspose.zip.wim/wimfileentry/open/)() | Opent het item voor extractie en biedt een stream met inhoud van het item. |
| override [ToString](../../aspose.zip.wim/wimentry/tostring/)() |  |

### Zie ook

* class [WimEntry](../wimentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* naamruimte [Aspose.Zip.Wim](../../aspose.zip.wim/)
* montage [Aspose.Zip](../../)


