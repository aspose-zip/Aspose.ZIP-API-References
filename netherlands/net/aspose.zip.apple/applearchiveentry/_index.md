---
title: "Klasse AppleArchiveEntry"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "Aspose.Zip.Apple.AppleArchiveEntry class. Vertegenwoordigt een bestandssysteemitem binnen een AppleArchive"
type: docs
weight: 70
url: /nl/net/aspose.zip.apple/applearchiveentry/
---
## AppleArchiveEntry class

Vertegenwoordigt een bestandssysteemitem binnen een [`AppleArchive`](../applearchive/).

```csharp
public sealed class AppleArchiveEntry : IArchiveFileEntry
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [IsDirectory](../../aspose.zip.apple/applearchiveentry/isdirectory/) { get; } | Haalt een waarde op die aangeeft of het item een map vertegenwoordigt. |
| [IsSymbolicLink](../../aspose.zip.apple/applearchiveentry/issymboliclink/) { get; } | Haalt een waarde op die aangeeft of het item een symbolische link vertegenwoordigt. |
| [Length](../../aspose.zip.apple/applearchiveentry/length/) { get; } | Haalt de ongecomprimeerde lengte van het item op in bytes. |
| [Name](../../aspose.zip.apple/applearchiveentry/name/) { get; } | Haalt het pad van het item binnen het archief op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract_1)(Stream) | Extraheert het item naar de opgegeven stream. |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract)(string) | Extraheert het item naar het bestandssysteem op het opgegeven pad. |
| [Open](../../aspose.zip.apple/applearchiveentry/open/)() | Opent het item voor extractie en biedt een stream met de inhoud van het item. |

## Opmerkingen

Een instantie van deze klasse kan een regulier bestand, een map of een symbolische link vertegenwoordigen die is geparseerd uit een bestaande Apple Archive, of een bestand of map die aan een te componeren archief wordt toegevoegd.

### Zie ook

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


