---
title: CreateEntry
second_title: Aspose.ZIP for .NET API Reference
description: 
type: docs
weight: 50
url: /net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## SevenZipArchive.CreateEntry method (1 of 4)

Create single entry within the archive.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| fileInfo | FileInfo | The metadata of file to be compressed. |
| openImmediately | Boolean | True if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | SevenZipEntrySettings | Compression and encryption settings used for added [`SevenZipArchiveEntry`](../../sevenziparchiveentry) item. |

### Return Value

Seven Zip entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* is read-only or is a directory. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| IOException | The file is already open. |

### Remarks

The entry name is solely set within *name* parameter. The file name provided in *fileInfo* parameter does not affect the entry name.

If the file is opened immediately with *openImmediately* parameter it becomes blocked until archive is saved.

### Examples

Compose archive with entries encrypted with different passwords each.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
        archive.CreateEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
        archive.CreateEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
        archive.Save(sevenZipFile);
    }
}
```

### See Also

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive.CreateEntry method (2 of 4)

Create single entry within the archive.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| source | Stream | The input stream for the entry. |
| newEntrySettings | SevenZipEntrySettings | Compression and encryption settings used for added [`SevenZipArchiveEntry`](../../sevenziparchiveentry) item. |
| fileInfo | FileSystemInfo | The metadata of file or folder to be compressed. |

### Return Value

SevenZip entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Both *source* and *fileInfo* are null or *source* is null and *fileInfo* stands for directory. |

### Remarks

The entry name is solely set within *name* parameter. The file name provided in *fileInfo* parameter does not affect the entry name.

*fileInfo* can refer to DirectoryInfo if the entry is directory.

### Examples

Compose archive with LZMA2 compressed encrypted entry.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF}), new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new FileInfo("data1.bin")); 
        archive.Save(sevenZipFile);
    }
}
```

### See Also

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive.CreateEntry method (3 of 4)

Create single entry within the archive.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| source | Stream | The input stream for the entry. |
| newEntrySettings | SevenZipEntrySettings | Compression and encryption settings used for added [`SevenZipArchiveEntry`](../../sevenziparchiveentry) item. |

### Return Value

Zip entry instance.

### Examples

Compose 7z archive with LZMA2 compression and encryption of all entries.

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### See Also

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive)
* assembly [Aspose.Zip](../../../)

---

## SevenZipArchive.CreateEntry method (4 of 4)

Create single entry within the archive.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| path | String | The fully qualified name of the new file, or the relative file name to be compressed. |
| openImmediately | Boolean | True if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | SevenZipEntrySettings | Compression and encryption settings used for added [`SevenZipArchiveEntry`](../../sevenziparchiveentry) item. |

### Return Value

Zip entry instance.

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

The entry name is solely set within *name* parameter. The file name provided in *path* parameter does not affect the entry name.

If the file is opened immediately with *openImmediately* parameter it becomes blocked until archive is saved.

### Examples

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings())))
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### See Also

* class [SevenZipArchiveEntry](../../sevenziparchiveentry)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings)
* class [SevenZipArchive](../../sevenziparchive)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive)
* assembly [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.ZIP.dll -->
