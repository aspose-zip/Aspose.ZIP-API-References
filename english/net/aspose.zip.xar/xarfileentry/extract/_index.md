---
title: XarFileEntry.Extract
second_title: Aspose.ZIP for .NET API Reference
description: XarFileEntry method. Extracts the entry to the filesystem by the path provided
type: docs
weight: 20
url: /net/aspose.zip.xar/xarfileentry/extract/
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
| InvalidDataException | Archive is corrupted. |

## Examples

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    ((XarFileEntry)archive.Entries[0]).Extract("data.bin");
}
```

### See Also

* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
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
| InvalidDataException | Archive is corrupted. |

## Examples

Extract an entry of xar archive.

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    ((XarFileEntry)archive.Entries[0]).Extract(httpResponseStream);
}
```

### See Also

* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


