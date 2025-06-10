---
title: LhaArchive.LhaArchive
second_title: Aspose.ZIP for .NET API Reference
description: LhaArchive constructor. Initializes a new instance of the LhaArchive class and composes an entry list can be extracted from the archive
type: docs
weight: 10
url: /net/aspose.zip.lha/lhaarchive/lhaarchive/
---
## LhaArchive(Stream, LhaLoadOptions) {#constructor}

Initializes a new instance of the [`LhaArchive`](../) class and composes an entry list can be extracted from the archive.

```csharp
public LhaArchive(Stream sourceStream, LhaLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | The source of the archive. |
| loadOptions | LhaLoadOptions | Options to load existing archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceStream* is null |
| ArgumentException | *sourceStream* is unseekable. |
| InvalidDataException | Inappropriate data found. |

## Remarks

This constructor does not decompress any entry. See [`Extract`](../../lhaarchiveentry/extract/) method for decompressing.

### See Also

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LhaArchive(string, LhaLoadOptions) {#constructor_1}

Initializes a new instance of the [`LhaArchive`](../) class and composes an entry list can be extracted from the archive.

```csharp
public LhaArchive(string path, LhaLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The fully qualified or the relative path to the archive file. |
| loadOptions | LhaLoadOptions | Options to load existing archive with. |

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

## Remarks

This constructor does not decompress any entry. See [`Extract`](../../lhaarchiveentry/extract/) method for decompressing.

## Examples

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LhaArchive archive = new LhaArchive("sample.lzh"))
{
    archive.Entries[0].Extract(extracted);
}
```

### See Also

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


