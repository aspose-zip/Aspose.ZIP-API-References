---
title: SevenZipArchiveEntry.Open
second_title: Aspose.ZIP for .NET API Reference
description: SevenZipArchiveEntry method. Opens the entry for extraction and provides a stream with entry content
type: docs
weight: 90
url: /net/aspose.zip.sevenzip/sevenziparchiveentry/open/
---
## SevenZipArchiveEntry.Open method

Opens the entry for extraction and provides a stream with entry content.

```csharp
public Stream Open(string password = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Optional password for decryption. |

### Return Value

The stream that represents the contents of the entry.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | The archive is not opened for extraction. - or - This entry is a directory. |
| InvalidDataException | Wrong data within the entry. |

## Remarks

Read from the stream to get the original content of a file. See examples section.

## Examples

Usage:

```csharp
Stream decompressed = entry.Open();
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

* class [SevenZipArchiveEntry](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* assembly [Aspose.Zip](../../../)


