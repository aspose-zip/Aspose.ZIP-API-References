---
title: CabEntry.Extract
second_title: Aspose.ZIP for .NET API Reference
description: CabEntry method. Extracts the entry to the filesystem by the path provided
type: docs
weight: 40
url: /net/aspose.zip.cab/cabentry/extract/
---
## Extract(string) {#extract}

Extracts the entry to the filesystem by the path provided.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to destination file. If the file already exists, it will be overwritten. |

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
| FileNotFoundException | The file is not found. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| IOException | The file is already open. |
| NotSupportedException | Stream initialization failed due to wrong data. |
| InvalidDataException | The archive is corrupted. |

## Examples

```csharp
using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### See Also

* class [CabEntry](../)
* namespace [Aspose.Zip.Cab](../../cabentry/)
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
| ArgumentException | *destination* does not support writing. |
| NotSupportedException | Stream initialization failed due to wrong data. |
| InvalidDataException | The archive is corrupted. |

## Examples

Extract an entry of cab archive.

```csharp
Using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### See Also

* class [CabEntry](../)
* namespace [Aspose.Zip.Cab](../../cabentry/)
* assembly [Aspose.Zip](../../../)


