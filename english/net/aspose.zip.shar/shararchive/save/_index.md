---
title: SharArchive.Save
second_title: Aspose.ZIP for .NET API Reference
description: SharArchive method. Saves archive to destination file provided
type: docs
weight: 70
url: /net/aspose.zip.shar/shararchive/save/
---
## Save(string) {#save_1}

Saves archive to destination file provided.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *destinationFileName* is a zero-length string, contains only white space, or contains one or more invalid characters as defined by System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* is null. |
| PathTooLongException | The specified *destinationFileName*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| DirectoryNotFoundException | The specified *destinationFileName* is invalid, (for example, it is on an unmapped drive). |
| IOException | An I/O error occurred while opening the file. |
| UnauthorizedAccessException | *destinationFileName* specified a file that is read-only and access is not Read.-or- path specified a directory.-or- The caller does not have the required permission. |
| NotSupportedException | *destinationFileName* is in an invalid format. |
| FileNotFoundException | The file is not found. |

## Remarks

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to temporary file.

## Examples

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.shar");
}       
```

### See Also

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream) {#save}

Saves archive to the stream provided.

```csharp
public void Save(Stream output)
```

| Parameter | Type | Description |
| --- | --- | --- |
| output | Stream | Destination stream. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *output* is null. |
| ArgumentException | *output* is not writable. - or - *output* is the same stream we extract from. |

## Remarks

*output* must be writable.

## Examples

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(sharFile);
    }
}       
```

### See Also

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


