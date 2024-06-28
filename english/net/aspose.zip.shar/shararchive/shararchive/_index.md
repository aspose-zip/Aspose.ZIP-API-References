---
title: SharArchive.SharArchive
second_title: Aspose.ZIP for .NET API Reference
description: SharArchive constructor. Initializes a new instance of the SharArchive class
type: docs
weight: 10
url: /net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

Initializes a new instance of the [`SharArchive`](../) class.

```csharp
public SharArchive()
```

## Examples

The following example shows how to compress a file.

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### See Also

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

Initializes a new instance of the [`SharArchive`](../) class prepared for decompressing.

```csharp
public SharArchive(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | Path to the source of the archive. |

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

### See Also

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


