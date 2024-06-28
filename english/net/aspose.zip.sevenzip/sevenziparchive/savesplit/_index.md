---
title: SevenZipArchive.SaveSplit
second_title: Aspose.ZIP for .NET API Reference
description: SevenZipArchive method. Saves multivolume archive to destination directory provided
type: docs
weight: 90
url: /net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

Saves multi-volume archive to destination directory provided.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | String | The path to the directory where archive segments to be created. |
| options | SplitSevenZipArchiveSaveOptions | Options for archive saving, including file name. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | This archive was opened from existing source. |
| ArgumentNullException | *destinationDirectory* is null. |
| SecurityException | The caller does not have the required permission to access the directory. |
| ArgumentException | *destinationDirectory* contains invalid characters such as ", &gt;, &lt;, or &#x7C;. |
| PathTooLongException | The specified path exceeds the system-defined maximum length. |

## Remarks

This method compose several (`n`) files filename.7z.001, filename.7z.002, ..., filename.7z.(n).

Can not make existing archive multi-volume.

## Examples

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### See Also

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


