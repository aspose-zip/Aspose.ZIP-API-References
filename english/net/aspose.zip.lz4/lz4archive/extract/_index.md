---
title: Lz4Archive.Extract
second_title: Aspose.ZIP for .NET API Reference
description: Lz4Archive method. Extracts the archive to the file by path
type: docs
weight: 30
url: /net/aspose.zip.lz4/lz4archive/extract/
---
## Extract(string) {#extract}

Extracts the archive to the file by path.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to destination file. If the file already exists, it will be overwritten. |

### Return Value

Info of an extracted file.

### Exceptions

| exception | condition |
| --- | --- |
| EndOfStreamException | Source stream is too short. |
| InvalidDataException | Wrong bytes found while decoding. |
| NotSupportedException | This LZ4 version is not supported. |

### See Also

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extracts the archive to the stream provided.

```csharp
public void Extract(Stream destination)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destination | Stream | Destination stream. Must be writable. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *destination* does not support writing. |
| EndOfStreamException | Source stream is too short. |
| InvalidDataException | Wrong bytes found while decoding. |
| NotSupportedException | This LZ4 version is not supported. |
| InvalidOperationException | The archive is prepared for composition. |

## Examples

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### See Also

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


