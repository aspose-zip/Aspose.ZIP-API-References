---
title: XarArchive.Save
second_title: Aspose.ZIP for .NET API Reference
description: XarArchive method. Saves archive to the destination file provided
type: docs
weight: 80
url: /net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

Saves archive to the destination file provided.

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| saveOptions | XarSaveOptions | Options to save xar archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationFileName* is null. |
| InvalidOperationException | Impossible to modify xar archive. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |
| IOException | An I/O error occurred while opening the file. |
| PathTooLongException | The specified path, file name, or both exceed the system-defined maximum length. |
| UnauthorizedAccessException | *destinationFileName* specified a file that is read-only. -or- *destinationFileName* specified a directory. -or- The caller does not have the required permission. |

### See Also

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

Saves archive to the stream provided.

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| output | Stream | Destination stream. |
| saveOptions | XarSaveOptions | Options to save xar archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *output* is null. |
| ArgumentException | *output*Is not writable/readable or not seekable. |
| InvalidOperationException | Impossible to modify xar archive. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

### See Also

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


