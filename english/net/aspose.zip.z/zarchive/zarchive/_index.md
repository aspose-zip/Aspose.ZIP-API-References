---
title: ZArchive.ZArchive
second_title: Aspose.ZIP for .NET API Reference
description: ZArchive constructor. Initializes a new instance of the ZArchive class prepared for compressing
type: docs
weight: 10
url: /net/aspose.zip.z/zarchive/zarchive/
---
## ZArchive() {#constructor}

Initializes a new instance of the [`ZArchive`](../) class prepared for compressing.

```csharp
public ZArchive()
```

### See Also

* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZArchive(Stream, ZArchiveLoadOptions) {#constructor_1}

Initializes a new instance of the [`ZArchive`](../) class prepared for decompressing.

```csharp
public ZArchive(Stream source, ZArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Stream | The source of the archive. |
| loadOptions | ZArchiveLoadOptions | The options to load archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *source* is not seekable. |
| ArgumentNullException | *source* is null. |

## Remarks

This constructor does not decompress. See [`Extract`](../extract/) method for decompressing.

### See Also

* class [ZArchiveLoadOptions](../../zarchiveloadoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZArchive(string, ZArchiveLoadOptions) {#constructor_2}

Initializes a new instance of the [`ZArchive`](../) class prepared for decompressing.

```csharp
public ZArchive(string path, ZArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | Path to the source of the archive. |
| loadOptions | ZArchiveLoadOptions | The options to load archive with. |

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

## Remarks

This constructor does not decompress. See [`Extract`](../extract/) method for decompressing.

### See Also

* class [ZArchiveLoadOptions](../../zarchiveloadoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)


