---
title: LzipArchive.Save
second_title: Aspose.ZIP for .NET API Reference
description: LzipArchive method. Saves lzip archive to the stream provided
type: docs
weight: 60
url: /net/aspose.zip.lzip/lziparchive/save/
---
## Save(Stream) {#save_1}

Saves lzip archive to the stream provided.

```csharp
public void Save(Stream outputStream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | Stream | Destination stream. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *outputStream* does not support seeking. |
| ArgumentNullException | *outputStream* is null. |

## Remarks

*outputStream* must be seekable.

## Examples

```csharp
using (FileStream lzFile = File.Open("archive.lz", FileMode.Create))
{
    using (var archive = new LzipArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(lzFile);
     }
}
```

### See Also

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Saves lzip archive to destination file provided.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationFileName* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *destinationFileName* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *destinationFileName* is denied. |
| PathTooLongException | The specified *destinationFileName*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *destinationFileName* contains a colon (:) in the middle of the string. |

## Examples

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lz");
}
```

### See Also

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Saves lzip archive to destination file provided.

```csharp
public void Save(FileInfo destination)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destination | FileInfo | FileInfo which will be opened as destination stream. |

### Exceptions

| exception | condition |
| --- | --- |
| SecurityException | The caller does not have the required permission to open the *destination*. |
| ArgumentException | File path is empty or contains only white spaces. |
| FileNotFoundException | The file is not found. |
| UnauthorizedAccessException | Path to file is read-only or is a directory. |
| ArgumentNullException | *destination* is null. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| IOException | The file is already open. |

## Examples

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz"));
}
```

### See Also

* class [LzipArchive](../)
* namespace [Aspose.Zip.Lzip](../../lziparchive/)
* assembly [Aspose.Zip](../../../)


