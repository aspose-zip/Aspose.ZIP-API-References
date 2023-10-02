---
title: ZArchive.Extract
second_title: Aspose.ZIP for .NET API Reference
description: ZArchive method. Extracts Z archive to a stream
type: docs
weight: 30
url: /net/aspose.zip.z/zarchive/extract/
---
## Extract(Stream) {#extract_2}

Extracts Z archive to a stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destination | Stream | Stream for storing decompressed data. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidDataException | Data can not be decompressed. |

## Examples

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new ZArchive(zFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### See Also

* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Extracts Z archive to a file.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo for storing decompressed data. |

### Exceptions

| exception | condition |
| --- | --- |
| SecurityException | The caller does not have the required permission to open the *fileInfo*. |
| ArgumentException | File path is empty or contains only white spaces. |
| FileNotFoundException | The file is not found. |
| UnauthorizedAccessException | Path to file is read-only or is a directory. |
| ArgumentNullException | *fileInfo* is null. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| IOException | The file is already open. |
| InvalidDataException | Data can not be decompressed. |

## Examples

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### See Also

* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Extracts Z archive to a file by path.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | Path to file which will store decompressed data. |

### Return Value

Info of extracted file.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* contains a colon (:) in the middle of the string. |
| InvalidDataException | Data can not be decompressed. |

## Examples

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### See Also

* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)


