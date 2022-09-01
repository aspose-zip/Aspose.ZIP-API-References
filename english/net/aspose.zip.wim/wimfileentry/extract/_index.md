---
title: Extract
second_title: Aspose.ZIP for .NET API Reference
description: 
type: docs
weight: 20
url: /net/aspose.zip.wim/wimfileentry/extract/
---
## WimFileEntry.Extract method (1 of 2)

Extracts the entry to the filesystem by the path provided.

```csharp
public FileSystemInfo Extract(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to destination file. If the file already exists, it will be overwritten. |

### Return Value

The file info of composed file.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* contains a colon (:) in the middle of the string. |

### Examples

```csharp
using (var archive = new WimArchive("archive.wim"))
{
    archive.Images[0].RootDirectory.Files[0].Extract("data.bin");
}
```

### See Also

* class [WimFileEntry](../../wimfileentry)
* namespace [Aspose.Zip.Wim](../../wimfileentry)
* assembly [Aspose.Zip](../../../)

---

## WimFileEntry.Extract method (2 of 2)

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

### Examples

Extract an entry of wim archive.

```csharp
using (var archive = new WimArchive("archive.wim"))
{
    archive.Images[0].RootDirectory.Files[0].Extract(httpResponseStream);
}
```

### See Also

* class [WimFileEntry](../../wimfileentry)
* namespace [Aspose.Zip.Wim](../../wimfileentry)
* assembly [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.ZIP.dll -->