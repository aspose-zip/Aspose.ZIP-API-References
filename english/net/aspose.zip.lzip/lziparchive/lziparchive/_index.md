---
title: LzipArchive.LzipArchive
second_title: Aspose.ZIP for .NET API Reference
description: LzipArchive constructor. Initializes a new instance of the LzipArchive
type: docs
weight: 10
url: /net/aspose.zip.lzip/lziparchive/lziparchive/
---
## LzipArchive(LzipArchiveSettings) {#constructor}

Initializes a new instance of the [`LzipArchive`](../).

```csharp
public LzipArchive(LzipArchiveSettings settings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| settings | LzipArchiveSettings | Setting of particular lzip archive with definition of dictionary size. |

### See Also

* class [LzipArchiveSettings](../../lziparchivesettings/)
* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## LzipArchive(Stream, LzipLoadOptions) {#constructor_1}

Initializes a new instance of the [`LzipArchive`](../) class prepared for decompressing.

```csharp
public LzipArchive(Stream sourceStream, LzipLoadOptions options = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | The source of the archive. |
| options | LzipLoadOptions | Options to load the archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *sourceStream* is not seekable. |
| ArgumentNullException | *sourceStream* is null. |
| InvalidDataException | Headers do not match lzip type of archive. |

## Remarks

This constructor does not decompress. See [`Extract`](../extract/) method for decompressing.

### See Also

* class [LzipLoadOptions](../../lziploadoptions/)
* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## LzipArchive(string, LzipLoadOptions) {#constructor_2}

Initializes a new instance of the [`LzipArchive`](../) class prepared for decompressing.

```csharp
public LzipArchive(string path, LzipLoadOptions options = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | Path to the source of the archive. |
| options | LzipLoadOptions | Options to load the archive with. |

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
| InvalidDataException | Headers do not match lzip type of archive. |

## Remarks

This constructor does not decompress. See [`Extract`](../extract/) method for decompressing.

## Examples

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new LzipArchive(sourceLzipFile))
    {
         archive.Extract(extractedFile);
       }
   }
```

### See Also

* class [LzipLoadOptions](../../lziploadoptions/)
* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)


