---
title: UueArchive.Open
second_title: Aspose.ZIP for .NET API Reference
description: UueArchive method. Opens the archive for decoding and provides a stream with archive content
type: docs
weight: 60
url: /net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

Opens the archive for decoding and provides a stream with archive content.

```csharp
public Stream Open()
```

### Return Value

The stream that represents the contents of the archive.

## Remarks

Read from the stream to get original content of file. See examples section.

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

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


