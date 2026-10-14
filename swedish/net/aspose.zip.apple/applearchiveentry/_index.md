---
title: "Klass AppleArchiveEntry"
second_title: "Aspose.ZIP för .NET API-referens"
description: "Aspose.Zip.Apple.AppleArchiveEntry klass. Representerar ett filsystemspost inom ett AppleArchive"
type: docs
weight: 70
url: /sv/net/aspose.zip.apple/applearchiveentry/
---
## AppleArchiveEntry class

Representerar ett filsystemspost inom ett [`AppleArchive`](../applearchive/).

```csharp
public sealed class AppleArchiveEntry : IArchiveFileEntry
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [IsDirectory](../../aspose.zip.apple/applearchiveentry/isdirectory/) { get; } | Hämtar ett värde som indikerar om posten representerar en katalog. |
| [IsSymbolicLink](../../aspose.zip.apple/applearchiveentry/issymboliclink/) { get; } | Hämtar ett värde som indikerar om posten representerar en symbolisk länk. |
| [Length](../../aspose.zip.apple/applearchiveentry/length/) { get; } | Hämtar den okomprimerade längden på posten i byte. |
| [Name](../../aspose.zip.apple/applearchiveentry/name/) { get; } | Hämtar sökvägen för posten i arkivet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract_1)(Stream) | Extraherar posten till den angivna strömmen. |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract)(string) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [Open](../../aspose.zip.apple/applearchiveentry/open/)() | Öppnar posten för extrahering och tillhandahåller en ström med postens innehåll. |

## Anmärkningar

En instans av denna klass kan representera en vanlig fil, katalog eller symbolisk länk som parsats från ett befintligt Apple Archive, eller en fil eller katalog som lagts till i ett arkiv som byggs.

### Se även

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


