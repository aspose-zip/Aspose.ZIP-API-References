---
title: ZstandardArchive.Open
second_title: Aspose.ZIP for .NET API Reference
description: ZstandardArchive method. Opens the archive for extraction and provides a stream with archive content
type: docs
weight: 50
url: /net/aspose.zip.zstandard/zstandardarchive/open/
---
## ZstandardArchive.Open method

Opens the archive for extraction and provides a stream with archive content.

```csharp
public Stream Open()
```

### Return Value

The stream that represents the contents of the archive.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Remarks

Read from the stream to get the original content of a file. See examples section.

## Examples

Extracts the archive and copies extracted content to file stream.

```csharp
using (var archive = new ZstandardArchive("archive.zst"))
{
    using (var extracted = File.Create("data.bin"))
    {
        var unpacked = archive.Open();
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }            
}
```

You may use Stream.CopyTo method for .NET 4.0 and higher:

```csharp
unpacked.CopyTo(extracted);
```

### See Also

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


