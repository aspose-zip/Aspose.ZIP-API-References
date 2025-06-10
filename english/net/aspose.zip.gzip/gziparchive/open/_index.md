---
title: GzipArchive.Open
second_title: Aspose.ZIP for .NET API Reference
description: GzipArchive method. Opens the archive for extraction and provides a stream with archive content
type: docs
weight: 70
url: /net/aspose.zip.gzip/gziparchive/open/
---
## GzipArchive.Open method

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
using (var archive = new GzipArchive("archive.gz"))
{
    using (var extracted = File.Create("data.bin"))
    {
        using(var unpacked = archive.Open())
        {
            byte[] b = new byte[8192];
            int bytesRead;
            while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
                extracted.Write(b, 0, bytesRead);
        }
    }            
}
```

You may use Stream.CopyTo method for .NET 4.0 and higher:

```csharp
unpacked.CopyTo(extracted);
```

### See Also

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


