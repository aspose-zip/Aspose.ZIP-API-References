---
title: CabArchive.Save
second_title: Aspose.ZIP for .NET API Reference
description: CabArchive method. Saves archive to the stream provided
type: docs
weight: 70
url: /net/aspose.zip.cab/cabarchive/save/
---
## Save(Stream, CabSaveOptions) {#save}

Saves archive to the stream provided.

```csharp
public void Save(Stream outputStream, CabSaveOptions saveOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | Stream | Destination stream. |
| saveOptions | CabSaveOptions | Options for archive saving. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *outputStream* is not writable. |
| ObjectDisposedException | The archive is disposed. |
| InvalidOperationException | The archive is prepared for extraction and cannot be saved. |

## Remarks

*outputStream* must be writable.

## Examples

```csharp
using (FileStream cabFile = File.Open("archive.cab", FileMode.Create))
{
    using (var archive = new CabArchive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(cabFile);
    }
}
```

### See Also

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, CabSaveOptions) {#save_1}

Saves archive to the destination file provided.

```csharp
public void Save(string destinationFileName, CabSaveOptions saveOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| saveOptions | CabSaveOptions | Options for archive saving. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationFileName* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *destinationFileName* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *destinationFileName* is denied. |
| PathTooLongException | The specified *destinationFileName*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *destinationFileName* contains a colon (:) in the middle of the string. |
| FileNotFoundException | The file is not found. |
| InvalidOperationException | The archive is opened for extraction. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| IOException | The file is already open. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Remarks

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file.

## Examples

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### See Also

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


