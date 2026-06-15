---
title: Class AppleArchive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Apple.AppleArchive class. This class represents an Apple Archive .aar file. Use it to compose Apple Archive files
type: docs
weight: 10
url: /net/aspose.zip.apple/applearchive/
---
## AppleArchive class

This class represents an Apple Archive (.aar) file. Use it to compose Apple Archive files.

```csharp
public class AppleArchive : IArchive
```

## Constructors

| Name | Description |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | Initializes a new instance of the `AppleArchive` class with settings used for composed entries. |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | Initializes a new instance of the `AppleArchive` class and composes an entry list can be extracted from the archive. |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | Initializes a new instance of the `AppleArchive` class and composes an entry list can be extracted from the archive. |

## Properties

| Name | Description |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | Gets entries constituting the archive. |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | Gets a value indicating whether the archive uses solid compression. In solid mode, all entry data is compressed as a single stream and individual entry extraction is not available. Use [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/) instead. |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | Gets settings used for newly composed entries. |

## Methods

| Name | Description |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | Adds to the archive all files and directories recursively in the directory given. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | Creates a single entry within the archive. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | Creates a single entry within the archive. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | Creates a single entry within the archive. |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | Extracts all the files in the archive to the directory provided. |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | Saves archive to the stream provided. |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | Saves archive to a destination file provided. |

## Remarks

Apple and Apple Archive are trademarks of Apple Inc.

### See Also

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


