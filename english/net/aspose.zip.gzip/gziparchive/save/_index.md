---
title: GzipArchive.Save
second_title: Aspose.ZIP for .NET API Reference
description: GzipArchive method. Saves archive to the stream provided
type: docs
weight: 80
url: /net/aspose.zip.gzip/gziparchive/save/
---
## Save(Stream) {#save}

Saves archive to the stream provided.

```csharp
public void Save(Stream outputStream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | Stream | Destination stream. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *outputStream* is not writable. |
| InvalidOperationException | Source has not been supplied. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Remarks

*outputStream* must be writable.

## Examples

Writes compressed data to http response stream.

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### See Also

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Saves archive to the destination file provided.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationFileName* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *destinationFileName* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *destinationFileName* is denied. |
| PathTooLongException | The specified *destinationFileName*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *destinationFileName* contains a colon (:) in the middle of the string. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Examples

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### See Also

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


