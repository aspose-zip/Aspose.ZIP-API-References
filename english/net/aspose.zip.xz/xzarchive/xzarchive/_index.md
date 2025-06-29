---
title: XzArchive.XzArchive
second_title: Aspose.ZIP for .NET API Reference
description: XzArchive constructor. Initializes a new instance of the XzArchive class and composes the archive in xz format
type: docs
weight: 10
url: /net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

Initializes a new instance of the [`XzArchive`](../) class and composes the archive in xz format.

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| settings | XzArchiveSettings | Set of setting particular xz archive: dictionary size, block size, check type. |

### See Also

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)

---

## XzArchive(Stream, XzLoadOptions) {#constructor_1}

Initializes a new instance of the [`XzArchive`](../) class prepared for decompressing.

```csharp
public XzArchive(Stream source, XzLoadOptions options = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Stream | The source of the archive. |
| options | XzLoadOptions | Options to load the archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *source* is not seekable. |
| ArgumentNullException | *source* is null. |

## Remarks

This constructor does not decompress. See [`Extract`](../extract/) method for decompressing.

### See Also

* class [XzLoadOptions](../../../aspose.zip.xz.settings/xzloadoptions/)
* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)

---

## XzArchive(string, XzLoadOptions) {#constructor_2}

Initializes a new instance of the [`XzArchive`](../) class prepared for decompressing.

```csharp
public XzArchive(string path, XzLoadOptions options = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | Path to the source of the archive. |
| options | XzLoadOptions | Options to load the archive with. |

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

* class [XzLoadOptions](../../../aspose.zip.xz.settings/xzloadoptions/)
* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)


