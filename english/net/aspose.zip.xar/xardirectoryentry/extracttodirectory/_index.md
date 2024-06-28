---
title: XarDirectoryEntry.ExtractToDirectory
second_title: Aspose.ZIP for .NET API Reference
description: XarDirectoryEntry method. Extracts all the files in the current directory to the directory provided
type: docs
weight: 50
url: /net/aspose.zip.xar/xardirectoryentry/extracttodirectory/
---
## XarDirectoryEntry.ExtractToDirectory method

Extracts all the files in the current directory to the directory provided.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | String | The path to the directory to place the extracted files in. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | path is null |
| PathTooLongException | The specified path, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters and file names must be less than 260 characters. |
| SecurityException | The caller does not have the required permission to access existing directory. |
| NotSupportedException | If directory does not exist, path contains a colon character (:) that is not part of a drive label ("C:\"). |
| ArgumentException | path is a zero-length string, contains only white space, or contains one or more invalid characters. You can query for invalid characters by using the System.IO.Path.GetInvalidPathChars method. -or- path is prefixed with, or contains, only a colon character (:). |
| IOException | The directory specified by path is a file. -or- The network name is not known. |
| InvalidDataException | Archive is corrupted. |

## Remarks

If the directory does not exist, it will be created.

## Examples

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   ((XarDirectoryEntry)archive.Entries[0]).ExtractToDirectory("C:\\extracted");
}
```

### See Also

* class [XarDirectoryEntry](../)
* namespace [Aspose.Zip.Xar](../../xardirectoryentry/)
* assembly [Aspose.Zip](../../../)


