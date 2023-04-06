---
title: Class CpioEntry
second_title: Aspose.ZIP för .NET API-referens
description: Aspose.Zip.Cpio.CpioEntry klass. Representerar en fil i cpioarkivet.
type: docs
weight: 170
url: /sv/net/aspose.zip.cpio/cpioentry/
---
## CpioEntry class

Representerar en fil i cpio-arkivet.

```csharp
public sealed class CpioEntry : IArchiveFileEntry
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [IsDirectory](../../aspose.zip.cpio/cpioentry/isdirectory/) { get; } | Får ett värde som indikerar om posten representerar katalog. |
| [LastWriteTimeUtc](../../aspose.zip.cpio/cpioentry/lastwritetimeutc/) { get; } | Får den senaste skrivtiden. |
| [Length](../../aspose.zip.cpio/cpioentry/length/) { get; } | Hämtar längden på posten i byte. |
| [Name](../../aspose.zip.cpio/cpioentry/name/) { get; } | Hämtar namnet på posten i arkivet. |
| [Parent](../../aspose.zip.cpio/cpioentry/parent/) { get; } | Hämtar arkivet som posten tillhör. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract_1)(Stream) | Extraherar posten till den tillhandahållna strömmen. |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract)(string) | Extraherar posten till filsystemet med den angivna sökvägen. |
| [Open](../../aspose.zip.cpio/cpioentry/open/)() | Öppnar posten för extraktion och tillhandahåller en ström med postinnehåll. |
| override [ToString](../../aspose.zip.cpio/cpioentry/tostring/)() |  |

### Se även

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namnutrymme [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* hopsättning [Aspose.Zip](../../)


