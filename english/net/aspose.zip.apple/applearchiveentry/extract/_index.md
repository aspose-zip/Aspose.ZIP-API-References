---
title: AppleArchiveEntry.Extract
second_title: Aspose.ZIP for .NET API Reference
description: AppleArchiveEntry method. Extracts the entry to the filesystem by the path provided
type: docs
weight: 40
url: /net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

Extracts the entry to the filesystem by the path provided.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to destination file. If the file already exists, it will be overwritten. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidDataException | The checksum or digest stored for the entry does not match the extracted data. |
| InvalidOperationException | The entry belongs to an archive prepared for composition, or the entry data cannot be opened from a non-seekable archive stream. |
| NotSupportedException | The entry belongs to a solid Apple Archive or uses an unsupported compression method. |
| ObjectDisposedException | The source stream has been disposed. |
| IOException | An I/O error occurs. |

### See Also

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extracts the entry to the stream provided.

```csharp
public void Extract(Stream destination)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destination | Stream | Destination stream. Must be writable. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destination* is `null`. |
| ArgumentException | *destination* does not support writing. |
| InvalidDataException | The checksum or digest stored for the entry does not match the extracted data. |
| InvalidOperationException | The entry belongs to an archive prepared for composition, or the entry data cannot be opened from a non-seekable archive stream. |
| NotSupportedException | The entry belongs to a solid Apple Archive or uses an unsupported compression method. |
| ObjectDisposedException | The source stream has been disposed. |
| IOException | An I/O error occurs. |

### See Also

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


