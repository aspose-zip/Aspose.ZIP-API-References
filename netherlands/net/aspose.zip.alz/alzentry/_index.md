---
title: "Klasse AlzEntry"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "Aspose.Zip.Alz.AlzEntry class. Vertegenwoordigt een bestand-item in een ALZ-archief met al zijn metadata"
type: docs
weight: 30
url: /nl/net/aspose.zip.alz/alzentry/
---
## AlzEntry class

Vertegenwoordigt een bestandsitem in een ALZ-archief met al zijn metadata.

```csharp
public abstract class AlzEntry : IArchiveFileEntry
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | Gecomprimeerde grootte van de bestandsgegevens in bytes. |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | Retourneert true als dit item een map vertegenwoordigt. |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | Bestandsnaam (zonder pad). |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | Niet‑gecomprimeerde grootte van de bestandsgegevens in bytes. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract_1)(Stream, string) | Extraheert het item naar de opgegeven stream. |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract)(string, string) | Extraheert het item naar het bestandssysteem op het opgegeven pad. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | Opent het item voor extractie en levert een stream met gedecomprimeerde inhoud van het item. |

### Zie ook

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


