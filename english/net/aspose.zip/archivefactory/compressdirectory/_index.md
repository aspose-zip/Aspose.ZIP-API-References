---
title: ArchiveFactory.CompressDirectory
second_title: Aspose.ZIP for .NET API Reference
description: ArchiveFactory method. Compresses the specified directory into an archive file using the provided archive format
type: docs
weight: 10
url: /net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

Compresses the specified directory into an archive file using the provided archive format.

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the directory that will be compressed. |
| outputFileName | String | Destination file name. |
| archiveFormat | ArchiveFormat | The format of the archive to create (e.g., zip, rar, tar, etc.). |

### Exceptions

| exception | condition |
| --- | --- |
| DirectoryNotFoundException | Thrown if the directory specified by *path* does not exist. |
| ArgumentException | Thrown if *path* is null or an empty string. |
| NotSupportedException | Thrown if the specified *archiveFormat* is not supported or recognized. |

## Remarks

This method will create an archive file at the location specified by the *path* parameter. The name of the archive file will typically be the directory name followed by the appropriate file extension based on the *archiveFormat*. The directory itself is not modified or deleted.

## Examples

Here is an example of how to use the CompressDirectory method:

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// This will create a zip file with the contents of the directory at the specified path.
```

### See Also

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


