---
title: SevenZipArchive.ExtractToDirectory
second_title: Aspose.ZIP for .NET API Reference
description: SevenZipArchive method. Extracts all the files in the archive to the directory provided
type: docs
weight: 70
url: /net/aspose.zip.sevenzip/sevenziparchive/extracttodirectory/
---
## SevenZipArchive.ExtractToDirectory method

Extracts all the files in the archive to the directory provided.

```csharp
public void ExtractToDirectory(string destinationDirectory, string password = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | String | The path to the directory to place the extracted files in. |
| password | String | Optional password for content decryption. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationDirectory* is null. |
| PathTooLongException | The specified path, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters and file names must be less than 260 characters. |
| SecurityException | The caller does not have the required permission to access existing directory. |
| NotSupportedException | If directory does not exist, path contains a colon character (:) that is not part of a drive label ("C:\"). |
| ArgumentException | *destinationDirectory* is a zero-length string, contains only white space, or contains one or more invalid characters. You can query for invalid characters by using the System.IO.Path.GetInvalidPathChars method. -or- path is prefixed with, or contains, only a colon character (:). |
| IOException | The directory specified by path is a file. -or- The network name is not known. |
| InvalidDataException | Archive is corrupted. |

## Remarks

If the directory does not exist, it will be created.

*password* is used for content decryption only. If file names are encrypted provide password in [`SevenZipArchive`](../sevenziparchive/) or [`SevenZipArchive`](../sevenziparchive/) constructor.

## Examples

```csharp
using (var archive = new SevenZipArchive("archive.7z")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### See Also

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


