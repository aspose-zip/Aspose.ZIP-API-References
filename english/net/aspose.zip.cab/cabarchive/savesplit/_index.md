---
title: CabArchive.SaveSplit
second_title: Aspose.ZIP for .NET API Reference
description: CabArchive method. Saves the archive as a linked set of CAB volumes in the destination directory
type: docs
weight: 80
url: /net/aspose.zip.cab/cabarchive/savesplit/
---
## CabArchive.SaveSplit method

Saves the archive as a linked set of CAB volumes in the destination directory.

```csharp
public void SaveSplit(string destinationDirectory, SplitCabSaveOptions saveOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | String | The existing directory where cabinet volumes will be created. |
| saveOptions | SplitCabSaveOptions | Options controlling volume names, size, checksums, and entry-source lifetime. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationDirectory* or *saveOptions* is null. |
| DirectoryNotFoundException | *destinationDirectory* does not exist. |
| IOException | A destination volume already exists or an I/O error occurs. |
| ObjectDisposedException | The archive has been disposed. |
| InvalidOperationException | The archive is prepared for extraction, or a CAB format limit is exceeded. |

## Remarks

For a file name of `volume`, this method creates volume1.cab, volume2.cab, ..., volume`n`.cab.

Existing volume files are not overwritten.

Volumes are written directly to their destination files without temporary files. Destination files may be incomplete until this method returns successfully. If saving fails, removal of volumes created by this call is attempted. Abrupt process termination may leave incomplete destination files.

## Examples

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder", new SplitCabSaveOptions("volume", 65536));
}
```

### See Also

* class [SplitCabSaveOptions](../../splitcabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


