---
title: LzxArchive.LzxArchive
second_title: Aspose.ZIP for .NET API Reference
description: LzxArchive constructor. Initializes a new instance of the LzxArchive class and composes an entry list can be extracted from the archive
type: docs
weight: 10
url: /net/aspose.zip.lzx/lzxarchive/lzxarchive/
---
## LzxArchive(Stream, LzxLoadOptions) {#constructor}

Initializes a new instance of the [`LzxArchive`](../) class and composes an entry list can be extracted from the archive.

```csharp
public LzxArchive(Stream extractionSource, LzxLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| extractionSource | Stream | The source of the archive. |
| loadOptions | LzxLoadOptions | Options to load existing archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *extractionSource* is null. |
| ArgumentException | *extractionSource* does not support seeking. |
| InvalidDataException | Wrong signature for archive. - or - The file is not a LZX archive. |
| NotImplementedException | Lzx archive contains merged entries. |
| EndOfStreamException | The *extractionSource* stream is too short. |

## Remarks

This constructor does not decompress any entry. See [`Extract`](../../lzxarchiveentry/extract/) method for decompressing.

### See Also

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzxArchive(string, LzxLoadOptions) {#constructor_1}

Initializes a new instance of the [`LzxArchive`](../) class and composes an entry list can be extracted from the archive.

```csharp
public LzxArchive(string path, LzxLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The fully qualified or the relative path to the archive file. |
| loadOptions | LzxLoadOptions | Options to load existing archive with. |

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
| InvalidDataException | The file is corrupted. |
| NotImplementedException | Lzx archive contains merged entries. |
| EndOfStreamException | The file is too short. |

## Remarks

This constructor does not decompress any entry. See [`Extract`](../../lzxarchiveentry/extract/) method for decompressing.

## Examples

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LzxArchive archive = new LzxArchive("sample.lzx"))
{
    archive.Entries[0].Extract(extracted);
}
```

### See Also

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


