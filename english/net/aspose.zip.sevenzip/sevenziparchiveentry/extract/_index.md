---
title: SevenZipArchiveEntry.Extract
second_title: Aspose.ZIP for .NET API Reference
description: SevenZipArchiveEntry method. Extracts the entry to the filesystem by the path provided
type: docs
weight: 80
url: /net/aspose.zip.sevenzip/sevenziparchiveentry/extract/
---
## Extract(string, string) {#extract}

Extracts the entry to the filesystem by the path provided.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to destination file. If the file already exists, it will be overwritten. |
| password | String | Optional password for decryption. |

### Return Value

The file info of a composed file.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* contains a colon (:) in the middle of the string. |
| InvalidDataException | The archive is corrupted. |

## Examples

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### See Also

* class [SevenZipArchiveEntry](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Extracts the entry to the stream provided.

```csharp
public void Extract(Stream destination, string password = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destination | Stream | Destination stream. Must be writable. |
| password | String | Optional password for decryption. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *destination* does not support writing. |
| InvalidOperationException | The archive is not opened for extraction. - or - This entry is a directory. |
| InvalidDataException | Wrong data within the entry. |

## Examples

Extract an entry of zip archive with password.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### See Also

* class [SevenZipArchiveEntry](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* assembly [Aspose.Zip](../../../)


