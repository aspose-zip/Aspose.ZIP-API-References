---
title: GzipArchive.Extract
second_title: Aspose.ZIP for .NET API Reference
description: GzipArchive method. Extracts the archive to the stream provided
type: docs
weight: 50
url: /net/aspose.zip.gzip/gziparchive/extract/
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
| InvalidDataException | Stream is corrupted and does not contain valid data. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |
| OperationCanceledException | In .NET Framework 4.0 and above: Thrown when the extraction is canceled via the provided cancellation token. |

## Examples

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
     archive.Extract(httpResponseStream);
}
```

### See Also

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

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

Info of extracted file.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* contains a colon (:) in the middle of the string. |
| InvalidDataException | Stream is corrupted and does not contain valid data. |
| OperationCanceledException | In .NET Framework 4.0 and above: Thrown when the extraction is canceled via the provided cancellation token. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

### See Also

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


