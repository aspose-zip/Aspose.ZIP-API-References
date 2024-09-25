---
title: Class CpioEntry
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Cpio.CpioEntry class. Represents single file within cpio archive
type: docs
weight: 180
url: /net/aspose.zip.cpio/cpioentry/
---
## CpioEntry class

Represents single file within cpio archive.

```csharp
public sealed class CpioEntry : IArchiveFileEntry
```

## Properties

| Name | Description |
| --- | --- |
| [IsDirectory](../../aspose.zip.cpio/cpioentry/isdirectory/) { get; } | Gets a value indicating whether the entry represents directory. |
| [LastWriteTimeUtc](../../aspose.zip.cpio/cpioentry/lastwritetimeutc/) { get; } | Gets the last write time. |
| [Length](../../aspose.zip.cpio/cpioentry/length/) { get; } | Gets the length of the entry in bytes. |
| [Name](../../aspose.zip.cpio/cpioentry/name/) { get; } | Gets name of the entry within archive. |
| [Parent](../../aspose.zip.cpio/cpioentry/parent/) { get; } | Gets the archive the entry belongs to. |

## Methods

| Name | Description |
| --- | --- |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract_1)(Stream) | Extracts the entry to the stream provided. |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract)(string) | Extracts the entry to the filesystem by the path provided. |
| [Open](../../aspose.zip.cpio/cpioentry/open/)() | Opens the entry for extraction and provides a stream with entry content. |
| override [ToString](../../aspose.zip.cpio/cpioentry/tostring/)() |  |

### See Also

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* assembly [Aspose.Zip](../../)


