---
title: Class XarFileEntry
second_title: Aspose.ZIP voor .NET API-referentie
description: Aspose.Zip.Xar.XarFileEntry klas. Vertegenwoordigt bestandsinvoer binnen xararchief.
type: docs
weight: 840
url: /nl/net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

Vertegenwoordigt bestandsinvoer binnen xar-archief.

```csharp
public abstract class XarFileEntry : XarEntry, IArchiveFileEntry
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | Krijgt de aanmaaktijd van het bestand of de map. |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | Krijgt het volledige pad van het item in het archief. |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | Krijgt een waarde die aangeeft of de vermelding een directory vertegenwoordigt. |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | Haalt de laatste toegangstijd van het bestand of de map op. |
| [LastWriteTime](../../aspose.zip.xar/xarentry/lastwritetime/) { get; } | Krijgt de wijzigingstijd van het bestand of de map. |
| abstract [Length](../../aspose.zip.xar/xarfileentry/length/) { get; } | Krijgt de lengte van het item in bytes. |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | Krijgt de naam van het item in het archief. |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | Haalt de bovenliggende map op waartoe het item behoort. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract_1)(Stream) | Extraheert de ingang van de geleverde stream. |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract)(string) | Extraheert de invoer naar het bestandssysteem via het opgegeven pad. |
| abstract [Open](../../aspose.zip.xar/xarfileentry/open/)() | Opent het item voor extractie en biedt een stream met inhoud van het item. |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

### Zie ook

* class [XarEntry](../xarentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* naamruimte [Aspose.Zip.Xar](../../aspose.zip.xar/)
* montage [Aspose.Zip](../../)


