---
title: Class ArjArchive
second_title: Aspose.ZIP for .NET API Reference
description: Aspose.Zip.Arj.ArjArchive class. This class represents an ARJ archive file
type: docs
weight: 100
url: /net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

This class represents an ARJ archive file.

```csharp
public class ArjArchive : IArchive
```

## Constructors

| Name | Description |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream) | Initializes a new instance of the `ArjArchive` class and composes an entry list can be extracted from the archive. |
| [ArjArchive](arjarchive/#constructor_1)(string) | Initializes a new instance of the `ArjArchive` class and composes an entry list can be extracted from the archive. |

## Properties

| Name | Description |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | Gets the commentary. |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | Gets entries of [`ArjEntryPlain`](../arjentryplain/) type constituting the ARJ archive. |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | Gets the original name. |

## Methods

| Name | Description |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | Extracts all entries to the specified directory. |

## Remarks

Only the following compression methods are supported:

**Method**

**Explanation**

**0**

Uncompressed

**1**

Combination of LZ77 and adaptive Huffman coding. Best ratio.

**2**

Combination of LZ77 and adaptive Huffman coding.

**3**

Combination of LZ77 and adaptive Huffman coding. Best speed.

### See Also

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


