---
title: Archive
second_title: Aspose.ZIP for .NET API Reference
description: 
type: docs
weight: 10
url: /net/aspose.zip/archive/archive/
---
## Archive constructor (1 of 4)

Initializes a new instance of the [`Archive`](../../archive) class with optional settings for its entries.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | Compression and encryption settings used for newly added [`ArchiveEntry`](../../archiveentry) items. If not specified, most common Deflate compression without encryption would be used. |

### Examples

The following example shows how to compress a single file with default settings.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### See Also

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* namespace [Aspose.Zip](../../archive)
* assembly [Aspose.Zip](../../../)

---

## Archive constructor (2 of 4)

Initializes a new instance of the [`Archive`](../../archive) class and composes entries list can be extracted from the archive.

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | The source of the archive. |
| loadOptions | ArchiveLoadOptions | Options to load existing archive with. |
| newEntrySettings | ArchiveEntrySettings | Compression and encryption settings used for newly added [`ArchiveEntry`](../../archiveentry) items. If not specified, most common Deflate compression without encryption would be used. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *sourceStream* is not seekable. |
| InvalidDataException | Encryption header for AES contradicts WinZip compression method. |

### Remarks

This constructor does not decompress any entry. See [`Open`](../../archiveentry/open) method for decompressing.

### Examples

The following example extract an encrypted archive, then decompress first entry to a `MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### See Also

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* namespace [Aspose.Zip](../../archive)
* assembly [Aspose.Zip](../../../)

---

## Archive constructor (3 of 4)

Initializes a new instance of the [`Archive`](../../archive) class and composes entries list can be extracted from the archive.

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The fully qualified or the relative path to the archive file. |
| loadOptions | ArchiveLoadOptions | Options to load existing archive with. |
| newEntrySettings | ArchiveEntrySettings | Compression and encryption settings used for newly added [`ArchiveEntry`](../../archiveentry) items. If not specified, most common Deflate compression without encryption would be used. |

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

This constructor does not decompress any entry. See [`Open`](../../archiveentry/open) method for decompressing.

### Examples

The following example extract an encrypted archive, then decompress first entry to a `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### See Also

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* namespace [Aspose.Zip](../../archive)
* assembly [Aspose.Zip](../../../)

---

## Archive constructor (4 of 4)

Initializes a new instance of the [`Archive`](../../archive) class from multi-volume zip archive and composes entries list can be extracted from the archive.

```csharp
public Archive(string mainSegment, string[] segmentsInOrder, ArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| mainSegment | String | Path to the last segment of multi-volume archive with the central directory. |
| segmentsInOrder | String[] | Paths to each segment but the last of multi-volume zip archive respecting order. |
| loadOptions | ArchiveLoadOptions | Options to load existing archive with. |

### Examples

This sample extract to a directory an archive of three segments.

```csharp
using (Archive a = new Archive("archive.zip", new string[] { "archive.z01", "archive.z02" }))
{
    a.ExtractToDirectory("destination");
}
```

### See Also

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [Archive](../../archive)
* namespace [Aspose.Zip](../../archive)
* assembly [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.ZIP.dll -->
