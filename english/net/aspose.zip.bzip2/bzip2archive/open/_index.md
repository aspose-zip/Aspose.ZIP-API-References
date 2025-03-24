---
title: Bzip2Archive.Open
second_title: Aspose.ZIP for .NET API Reference
description: Bzip2Archive method. Opens the archive for extraction and provides a stream with archive content
type: docs
weight: 50
url: /net/aspose.zip.bzip2/bzip2archive/open/
---
## Bzip2Archive.Open method

Opens the archive for extraction and provides a stream with archive content.

```csharp
public Stream Open()
```

### Return Value

The stream that represents the contents of the archive.

## Remarks

Read from the stream to get the original content of the file. See examples section.

## Examples

Usage:

```csharp
Stream decompressed = archive.Open();
```

.NET 4.0 and higher - use Stream.CopyTo method:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 and before - copy bytes manually:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

### See Also

* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


