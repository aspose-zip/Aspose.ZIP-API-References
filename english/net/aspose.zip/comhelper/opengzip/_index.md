---
title: ComHelper.OpenGzip
second_title: Aspose.ZIP for .NET API Reference
description: ComHelper method. Allows a COM application to load a gzip archive from a stream
type: docs
weight: 30
url: /net/aspose.zip/comhelper/opengzip/
---
## OpenGzip(Stream) {#opengzip}

Allows a COM application to load a gzip archive from a stream.

```csharp
public GzipArchive OpenGzip(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | A .NET stream object that contains the archive to load. |

### Return Value

A [`GzipArchive`](../../../aspose.zip.gzip/gziparchive/) object that represents the archive.

### Exceptions

| exception | condition |
| --- | --- |
| EndOfStreamException | Thrown when the end of the stream is reached before the expected number of bytes are read. |
| ArgumentNullException | Thrown when an *stream* is null. |
| InvalidDataException | Thrown when the data is invalid or corrupted. |

### See Also

* class [GzipArchive](../../../aspose.zip.gzip/gziparchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenGzip(string) {#opengzip_1}

Allows a COM application to load a gzip archive from a file.

```csharp
public GzipArchive OpenGzip(string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | Filename of the archive to load. |

### Return Value

A [`GzipArchive`](../../../aspose.zip.gzip/gziparchive/) object that represents the archive.

### Exceptions

| exception | condition |
| --- | --- |
| EndOfStreamException | Thrown when the end of the stream is reached before the expected number of bytes are read. |
| ArgumentException | The file name is empty, contains only white spaces, or contains invalid characters. |
| ArgumentNullException | *fileName* is `null`. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| FileNotFoundException | The file is not found. |
| InvalidDataException | Thrown when the data is invalid or corrupted. |
| PathTooLongException | The specified path, file name, or both exceed the system-defined maximum length. |
| UnauthorizedAccessException | Access to *fileName* is denied. |

### See Also

* class [GzipArchive](../../../aspose.zip.gzip/gziparchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


