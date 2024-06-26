---
title: LzmaArchive.LzmaArchive
second_title: Aspose.ZIP for .NET API Reference
description: LzmaArchive constructor. Initializes a new instance of the LzmaArchive class and composes the archive in lzma format
type: docs
weight: 10
url: /net/aspose.zip.lzma/lzmaarchive/lzmaarchive/
---
## LzmaArchive(LzmaArchiveSettings) {#constructor}

Initializes a new instance of the [`LzmaArchive`](../) class and composes the archive in lzma format.

```csharp
public LzmaArchive(LzmaArchiveSettings settings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| settings | LzmaArchiveSettings | Set of setting particular lzma archive. |

### See Also

* class [LzmaArchiveSettings](../../lzmaarchivesettings/)
* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzmaArchive(Stream) {#constructor_1}

Initializes a new instance of the [`LzmaArchive`](../) class prepared for decompressing.

```csharp
public LzmaArchive(Stream source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Stream | The source of the archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *source* is not seekable. |
| ArgumentNullException | *source* is null. |

## Remarks

This constructor does not decompress. See [`Extract`](../extract/) method for decompressing.

### See Also

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzmaArchive(string) {#constructor_2}

Initializes a new instance of the [`LzmaArchive`](../) class prepared for decompressing.

```csharp
public LzmaArchive(string path)
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

## Remarks

This constructor does not decompress. See [`Extract`](../extract/) method for decompressing.

## Examples

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzmaArchive(sourceLzmaFile))
    {
         archive.Extract(extractedFile);
    }
}
```

### See Also

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)


