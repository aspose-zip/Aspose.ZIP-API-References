---
title: LzmaArchive.Extract
second_title: Aspose.ZIP for .NET API Reference
description: LzmaArchive method. Extracts lzma archive to a stream
type: docs
weight: 30
url: /net/aspose.zip.lzma/lzmaarchive/extract/
---
## Extract(Stream) {#extract_1}

Extracts lzma archive to a stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destination | Stream | Stream for storing decompressed data. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Archive headers and service information were not read. |
| InvalidDataException | Error in data in header or checksum. |
| ArgumentNullException | Destination stream is null. |
| ArgumentException | Destination stream does not support writing. |

## Examples

```csharp
using (FileStream sourceLzmaFile = File.Open(sourceFileName, FileMode.Open))
{
   using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
   {
       using (var archive = new LzmaArchive(sourceLzmaFile))
       {
           archive.Extract(extractedFile);
       }
   }
}
```

### See Also

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract}

Extracts lzma archive to a file.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo for storing decompressed data. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Archive headers and service information were not read. |
| SecurityException | The caller does not have the required permission to open the *fileInfo*. |
| ArgumentException | File path is empty or contains only white spaces. |
| FileNotFoundException | The file is not found. |
| UnauthorizedAccessException | Path to file is read-only or is a directory. |
| ArgumentNullException | *fileInfo* is null. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| IOException | The file is already open. |

## Examples

```csharp
using (FileStream lzmaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzmaArchive(lzmaFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### See Also

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract_2}

Extracts lzma archive to a file by path.

```csharp
public void Extract(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | Path to file which will store decompressed data. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Archive headers and service information were not read. |
| ArgumentNullException | *path* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* contains a colon (:) in the middle of the string. |

## Examples

```csharp
using (FileStream lzmaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzmaArchive(lzmaFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### See Also

* class [LzmaArchive](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchive/)
* assembly [Aspose.Zip](../../../)


