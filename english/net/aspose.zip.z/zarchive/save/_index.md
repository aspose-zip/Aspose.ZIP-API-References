---
title: ZArchive.Save
second_title: Aspose.ZIP for .NET API Reference
description: ZArchive method. Saves xz archive to the stream provided
type: docs
weight: 50
url: /net/aspose.zip.z/zarchive/save/
---
## Save(Stream, ZArchiveSaveOptions) {#save}

Saves xz archive to the stream provided.

```csharp
public void Save(Stream output, ZArchiveSaveOptions settings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| output | Stream | Destination stream. |
| settings | ZArchiveSaveOptions | Optional settings for archive composition. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *output* does not support seeking. |
| ArgumentNullException | *output* is null. |

## Remarks

*output* must be seekable.

## Examples

```csharp
using (FileStream zFile = File.Open("data.bin.z", FileMode.Create))
{
    using (var archive = new ZArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(zFile);
     }
}
```

### See Also

* class [ZArchiveSaveOptions](../../zarchivesaveoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZArchiveSaveOptions) {#save_1}

Saves Z archive to the destination file provided.

```csharp
public void Save(string destinationFileName, ZArchiveSaveOptions settings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | String | +The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| settings | ZArchiveSaveOptions | Optional settings for archive composition. |

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
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### See Also

* class [ZArchiveSaveOptions](../../zarchivesaveoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)


