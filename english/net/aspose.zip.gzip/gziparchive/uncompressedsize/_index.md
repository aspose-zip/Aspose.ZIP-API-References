---
title: GzipArchive.UncompressedSize
second_title: Aspose.ZIP for .NET API Reference
description: GzipArchive property. Gets size of an original file
type: docs
weight: 30
url: /net/aspose.zip.gzip/gziparchive/uncompressedsize/
---
## GzipArchive.UncompressedSize property

Gets size of an original file.

```csharp
public ulong UncompressedSize { get; }
```

## Remarks

During decompression, this property may contain incorrect size. If the uncompressed file size exceeds 4GB, this property will give a wrong value due to the 32-bit limit in header.

### See Also

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


