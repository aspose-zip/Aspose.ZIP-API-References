---
title: Archive.SaveSplit
second_title: Aspose.ZIP for .NET API Reference
description: Archive method. Saves multivolume archive to destination directory provided
type: docs
weight: 110
url: /net/aspose.zip/archive/savesplit/
---
## SaveSplit(string, SplitArchiveSaveOptions) {#savesplit_1}

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
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |

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

---

## SaveSplit(IVolumeStreamProvider, SplitArchiveSaveOptions) {#savesplit}

Saves a multi-volume archive to streams supplied by a volume provider.

```csharp
public void SaveSplit(IVolumeStreamProvider volumeStreamProvider, SplitArchiveSaveOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| volumeStreamProvider | IVolumeStreamProvider | The provider of destination streams for the archive volumes. |
| options | SplitArchiveSaveOptions | Options for archive saving. [`FileName`](../../../aspose.zip.saving/splitarchivesaveoptions/filename/) is ignored. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *volumeStreamProvider* or *options* is null. |
| InvalidOperationException | This archive was opened from an existing source, or the provider returns a null or non-writable stream. |
| NotSupportedException | The archive uses XZ compression. |
| ObjectDisposedException | The archive is disposed. |

## Remarks

The supplied streams do not need to support seeking.

Each completed volume is flushed, passed to [`VolumeCompleted`](../../../aspose.zip.saving/ivolumestreamprovider/volumecompleted/), and then disposed.

Cannot make an existing archive multi-volume. XZ compression is not supported by this overload because it requires seeking.

## Examples

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(provider,  new SplitArchiveSaveOptions("volume", 65536));
}
```

### See Also

* interface [IVolumeStreamProvider](../../../aspose.zip.saving/ivolumestreamprovider/)
* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


