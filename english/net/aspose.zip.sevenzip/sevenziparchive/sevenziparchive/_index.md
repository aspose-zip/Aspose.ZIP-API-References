---
title: SevenZipArchive
second_title: Aspose.ZIP for .NET API Reference
description: 
type: docs
weight: 10
url: /net/aspose.zip.sevenzip/sevenziparchive/sevenziparchive/
---
## SevenZipArchive constructor (1 of 4)

Initializes a new instance of the [`SevenZipArchive`](../../sevenziparchive) class with optional settings for its entries.

```csharp
public SevenZipArchive(SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| newEntrySettings | SevenZipEntrySettings | Compression and encryption settings used for newly added [`SevenZipArchiveEntry`](../../sevenziparchiveentry) items. If not specified, LZMA compression without encryption would be used. |

### Examples

The following example shows how to compress a single file with default settings: LZMA compression without encryption.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### See Also

* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive constructor (2 of 4)

Initializes a new instance of the [`SevenZipArchive`](../../sevenziparchive) class and composes entries list can be extracted from the archive.

```csharp
public SevenZipArchive(Stream sourceStream, string password = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | The source of the archive. |
| password | String | Optional password for decryption. If file names are encrypted it must be present. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *sourceStream* is not seekable. |
| ArgumentNullException | *sourceStream* is null. |
| NotImplementedException | Archive contains more than one coder. Now only LZMA compression supported. |

### Remarks

This constructor does not decompress any entry. See [`ExtractToDirectory`](../extracttodirectory) method for decompressing.

### Examples

```csharp
using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z")))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### See Also

* class [SevenZipArchive](../../sevenziparchive)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive constructor (3 of 4)

Initializes a new instance of the [`SevenZipArchive`](../../sevenziparchive) class and composes entries list can be extracted from the archive.

```csharp
public SevenZipArchive(string path, string password = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The fully qualified or the relative path to the archive file. |
| password | String | Optional password for decryption. If file names are encrypted it must be present. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* contains a colon (:) in the middle of the string. |

### Remarks

This constructor does not decompress any entry. See [`ExtractToDirectory`](../extracttodirectory) method for decompressing.

### Examples

```csharp
using (SevenZipArchive archive = new SevenZipArchive("archive.7z"))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### See Also

* class [SevenZipArchive](../../sevenziparchive)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive constructor (4 of 4)

Initializes a new instance of the [`SevenZipArchive`](../../sevenziparchive) class from multi-volume 7z archive and composes entries list can be extracted from the archive.

```csharp
public SevenZipArchive(string[] parts, string password = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| parts | String[] | Paths to each segment of multi-volume 7z archive respecting order |
| password | String | Optional password for decryption. If file names are encrypted it must be present. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *parts* is null. |
| ArgumentException | *parts* has no entries. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The path to a file is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to a file is denied. |
| PathTooLongException | The specified path to a part, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at path contains a colon (:) in the middle of the string. |

### Examples

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new string[] { "multi.7z.001", "multi.7z.002", "multi.7z.003" } ))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### See Also

* class [SevenZipArchive](../../sevenziparchive)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive)
* assembly [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.ZIP.dll -->
