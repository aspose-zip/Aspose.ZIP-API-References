---
title: IsoArchive.Save
second_title: Aspose.ZIP for .NET API Reference
description: IsoArchive method. Saves the ISO image to the specified path
type: docs
weight: 80
url: /net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

Saves the ISO image to the specified path.

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path where the ISO image will be saved. |
| saveOptions | IsoSaveOptions | Options to save ISO archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Thrown when the archive is not in editing mode. |
| ArgumentNullException | Thrown when the *path* is null. |
| DirectoryNotFoundException | Thrown when the specified path is invalid, such as being on an unmapped drive. |
| IOException | Thrown when the file is already open. |
| UnauthorizedAccessException | Thrown when access to the file *path* is denied. |
| PathTooLongException | Thrown when the specified *path* exceeds the system-defined maximum length. |

## Examples

The following example shows how to save an ISO archive to a file:

```csharp
// Create a new empty ISO archive
using(IsoArchive isoArchive = new IsoArchive())
{
    // Add files to the ISO archive
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Save the ISO archive to a file
    isoArchive.Save("new_archive.iso");
}
```

### See Also

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

Saves the ISO image to the specified stream.

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream where the ISO image will be saved. |
| saveOptions | IsoSaveOptions | Options to save ISO archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Thrown when the archive is not in editing mode. |
| ArgumentNullException | Thrown when the *stream* is null. |
| ArgumentException | Thrown when the *stream* is not writable. |

## Examples

The following example shows how to save an ISO archive to a memory stream:

```csharp

 // Create a new empty ISO archive
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // Add files to the ISO archive
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // Save the ISO archive to a memory stream
     isoArchive.Save(memoryStream);
 }
```

### See Also

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


