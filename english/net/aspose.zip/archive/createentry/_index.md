---
title: Archive.CreateEntry
second_title: Aspose.ZIP for .NET API Reference
description: Archive method. Create single entry within the archive
type: docs
weight: 50
url: /net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_4}

Create single entry within the archive.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| path | String | The fully qualified name of the new file, or the relative file name to be compressed. |
| openImmediately | Boolean | True if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | ArchiveEntrySettings | Compression and encryption settings used for added [`ArchiveEntry`](../../archiveentry/) item. |

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

## Remarks

The entry name is solely set within *name* parameter. The file name provided in *path* parameter does not affect the entry name.

If the file is opened immediately with *openImmediately* parameter it becomes blocked until archive is saved.

## Examples

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

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_2}

Create single entry within the archive.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| source | Stream | The input stream for the entry. |
| newEntrySettings | ArchiveEntrySettings | Compression and encryption settings used for added [`ArchiveEntry`](../../archiveentry/) item. |

### Return Value

Zip entry instance.

## Examples

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### See Also

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry_1}

Create single entry within the archive.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| fileInfo | FileInfo | The metadata of file to be compressed. |
| openImmediately | Boolean | True if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | ArchiveEntrySettings | Compression and encryption settings used for added [`ArchiveEntry`](../../archiveentry/) item. |

### Return Value

Zip entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* is read-only or is a directory. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| IOException | The file is already open. |

## Remarks

The entry name is solely set within *name* parameter. The file name provided in *fileInfo* parameter does not affect the entry name.

If the file is opened immediately with *openImmediately* parameter it becomes blocked until archive is saved.

## Examples

Compose archive with entries encrypted with different encryption methods and passwords each.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
        archive.CreateEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass2", EncryptionMethod.AES128)));
        archive.CreateEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass3", EncryptionMethod.AES256)));
        archive.Save(zipFile);
    }
}
```

### See Also

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_3}

Create single entry within the archive.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| source | Stream | The input stream for the entry. |
| newEntrySettings | ArchiveEntrySettings | Compression and encryption settings used for added [`ArchiveEntry`](../../archiveentry/) item. |
| fileInfo | FileSystemInfo | The metadata of file or folder to be compressed. |

### Return Value

Zip entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Both *source* and *fileInfo* are null or *source* is null and *fileInfo* stands for directory. |

## Remarks

The entry name is solely set within *name* parameter. The file name provided in *fileInfo* parameter does not affect the entry name.

*fileInfo* can refer to DirectoryInfo if the entry is directory.

## Examples

Compose archive with encrypted entry.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF} ), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new FileInfo("data1.bin")); 
        archive.Save(zipFile);
    }
}
```

### See Also

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, ArchiveEntrySettings) {#createentry}

Create single entry within the archive.

```csharp
public ArchiveEntry CreateEntry(string name, Func<Stream> streamProvider, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| streamProvider | Func`1 | The method providing input stream for the entry. |
| newEntrySettings | ArchiveEntrySettings | Compression and encryption settings used for added [`ArchiveEntry`](../../archiveentry/) item. |

### Return Value

Zip entry instance.

## Remarks

This method is for .NET Framework 4.0 and above and for .NET Standard 2.0 version.

## Examples

Compose archive with encrypted entry.

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", provider, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")))); 
        archive.Save(zipFile);
    }
}
```

### See Also

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


