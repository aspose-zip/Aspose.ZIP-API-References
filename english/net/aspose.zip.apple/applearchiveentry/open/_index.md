---
title: AppleArchiveEntry.Open
second_title: Aspose.ZIP for .NET API Reference
description: AppleArchiveEntry method. Opens the entry for extraction and provides a stream with the entry content
type: docs
weight: 50
url: /net/aspose.zip.apple/applearchiveentry/open/
---
## AppleArchiveEntry.Open method

Opens the entry for extraction and provides a stream with the entry content.

```csharp
public Stream Open()
```

### Return Value

A readable stream that contains the extracted entry data.

### Exceptions

| exception | condition |
| --- | --- |
| NotSupportedException | The entry belongs to a solid Apple Archive or uses an unsupported compression method. |
| InvalidDataException | The checksum or digest stored for the entry does not match the extracted data. |
| InvalidOperationException | The entry belongs to an archive prepared for composition, or the entry data cannot be opened from a non-seekable archive stream. |
| ObjectDisposedException | The source stream has been disposed. |
| IOException | An I/O error occurs. |

## Remarks

Read from the returned stream to obtain the original entry content. If the archive contains checksum fields, the checksum is verified while the returned stream is read.

### See Also

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


