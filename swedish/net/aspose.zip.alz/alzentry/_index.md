---
title: "Klass AlzEntry"
second_title: "Aspose.ZIP för .NET API-referens"
description: "Aspose.Zip.Alz.AlzEntry-klass. Representerar en filpost i ett ALZ-arkiv med all dess metadata"
type: docs
weight: 30
url: /sv/net/aspose.zip.alz/alzentry/
---
## AlzEntry class

Representerar en filpost i ett ALZ-arkiv med all dess metadata.

```csharp
public abstract class AlzEntry : IArchiveFileEntry
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | Komprimerad storlek på fildata i byte. |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | Returnerar true om denna post representerar en katalog. |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | Filnamn (utan sökväg). |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | Okomprimerad storlek på fildata i byte. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract_1)(Stream, string) | Extraherar posten till den angivna strömmen. |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract)(string, string) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | Öppnar posten för extrahering och tillhandahåller en ström med dekomprimerat postinnehåll. |

### Se även

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


