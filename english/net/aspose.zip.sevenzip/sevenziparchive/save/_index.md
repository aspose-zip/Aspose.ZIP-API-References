---
title: SevenZipArchive.Save
second_title: Aspose.ZIP for .NET API Reference
description: SevenZipArchive method. Saves 7z archive to the stream provided
type: docs
weight: 80
url: /net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream, SevenZipArchiveSaveOptions) {#save}

Saves 7z archive to the stream provided.

```csharp
public void Save(Stream output, SevenZipArchiveSaveOptions saveOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| output | Stream | Destination stream. |
| saveOptions | SevenZipArchiveSaveOptions | Options for archive saving. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *output* does not support seeking. |
| ArgumentNullException | *output* is null. |
| InvalidOperationException | Encoder failed to compress data. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Remarks

*output* must be seekable.

## Examples

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
    using (var archive = new SevenZipArchive())
    {
      archive.CreateEntry("data", source);
      archive.Save(sevenZipFile);
    }
  }
}
```

### See Also

* class [SevenZipArchiveSaveOptions](../../../aspose.zip.saving/sevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, SevenZipArchiveSaveOptions) {#save_1}

Saves archive to a destination file provided.

```csharp
public void Save(string destinationFileName, SevenZipArchiveSaveOptions saveOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| saveOptions | SevenZipArchiveSaveOptions | Options for archive saving. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationFileName* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *destinationFileName* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *destinationFileName* is denied. |
| PathTooLongException | The specified *destinationFileName*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *destinationFileName* contains a colon (:) in the middle of the string. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Remarks

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file.

## Examples

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
   using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
   {
      archive.CreateEntry("data", source);
      archive.Save("archive.7z");
   }
}
```

### See Also

* class [SevenZipArchiveSaveOptions](../../../aspose.zip.saving/sevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


