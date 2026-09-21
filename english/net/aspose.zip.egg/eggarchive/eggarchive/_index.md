---
title: EggArchive.EggArchive
second_title: Aspose.ZIP for .NET API Reference
description: EggArchive constructor. Initializes a new instance of the EggArchive class from a stream
type: docs
weight: 10
url: /net/aspose.zip.egg/eggarchive/eggarchive/
---
## EggArchive(Stream, EggArchiveLoadOptions) {#constructor}

Initializes a new instance of the [`EggArchive`](../) class from a stream.

```csharp
public EggArchive(Stream stream, EggArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The EGG archive stream. The stream must support reading and seeking. |
| loadOptions | EggArchiveLoadOptions | Options to load the archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *stream* is null. |
| ArgumentException | *stream* is not readable and seekable. |

### See Also

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)

---

## EggArchive(string, EggArchiveLoadOptions) {#constructor_1}

Initializes a new instance of the [`EggArchive`](../) class from a file path.

```csharp
public EggArchive(string path, EggArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | Path to the EGG archive file. |
| loadOptions | EggArchiveLoadOptions | Options to load the archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* is null. |
| FileNotFoundException | The file does not exist. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* contains a colon (:) in the middle of the string. |
| FileNotFoundException | The file is not found. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| IOException | The file is already open. |

### See Also

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)


