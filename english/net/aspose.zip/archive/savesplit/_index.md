---
title: Archive.SaveSplit
second_title: Aspose.ZIP for .NET API Reference
description: Archive method. Saves multivolume archive to destination directory provided
type: docs
weight: 100
url: /net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

Saves multi-volume archive to destination directory provided.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | String | The path to the directory where archive segments to be created. |
| options | SplitArchiveSaveOptions | Options for archive saving, including file name. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | This archive was opened from the existing source. |
| NotSupportedException | This archive is both compressed with XZ method and encrypted. |
| ArgumentNullException | *destinationDirectory* is null. |
| SecurityException | The caller does not have the required permission to access the directory. |
| ArgumentException | *destinationDirectory* contains invalid characters such as ", &gt;, &lt;, or &#x7C;. |
| PathTooLongException | The specified path exceeds the system-defined maximum length. |
| ObjectDisposedException | The archive is disposed. |

## Remarks

This method composes several (`n`) files filename.z01, filename.z02, ..., filename.z(n-1), filename.zip.

Cannot make existing archive multi-volume.

## Examples

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### See Also

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


