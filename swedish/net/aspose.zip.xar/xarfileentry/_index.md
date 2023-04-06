---
title: Class XarFileEntry
second_title: Aspose.ZIP för .NET API-referens
description: Aspose.Zip.Xar.XarFileEntry klass. Representerar filpost i xararkivet.
type: docs
weight: 840
url: /sv/net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

Representerar filpost i xar-arkivet.

```csharp
public abstract class XarFileEntry : XarEntry, IArchiveFileEntry
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | Hämtar skapandet av filen eller katalogen. |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | Får fullständig sökväg till posten i arkivet. |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | Får ett värde som indikerar om posten representerar katalog. |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | Får den senaste åtkomsttiden för filen eller katalogen. |
| [LastWriteTime](../../aspose.zip.xar/xarentry/lastwritetime/) { get; } | Hämtar ändringstiden för filen eller katalogen. |
| abstract [Length](../../aspose.zip.xar/xarfileentry/length/) { get; } | Hämtar längden på posten i byte. |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | Hämtar namnet på posten i arkivet. |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | Hämtar den överordnade katalogen som posten tillhör. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract_1)(Stream) | Extraherar posten till den tillhandahållna strömmen. |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract)(string) | Extraherar posten till filsystemet med den angivna sökvägen. |
| abstract [Open](../../aspose.zip.xar/xarfileentry/open/)() | Öppnar posten för extraktion och tillhandahåller en ström med postinnehåll. |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

### Se även

* class [XarEntry](../xarentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namnutrymme [Aspose.Zip.Xar](../../aspose.zip.xar/)
* hopsättning [Aspose.Zip](../../)


