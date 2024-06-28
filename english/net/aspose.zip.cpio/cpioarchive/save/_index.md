---
title: CpioArchive.Save
second_title: Aspose.ZIP for .NET API Reference
description: CpioArchive method. Saves archive to destination file provided
type: docs
weight: 80
url: /net/aspose.zip.cpio/cpioarchive/save/
---
## Save(string, CpioFormat) {#save_1}

Saves archive to destination file provided.

```csharp
public void Save(string destinationFileName, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| cpioFormat | CpioFormat | Defines cpio header format. |

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

## Remarks

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to temporary file.

## Examples

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.cpio");
}       
```

### See Also

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, CpioFormat) {#save}

Saves archive to the stream provided.

```csharp
public void Save(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Type | Description |
| --- | --- | --- |
| output | Stream | Destination stream. |
| cpioFormat | CpioFormat | Defines cpio header format. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *output* is null. |
| ArgumentException | *output* is not writable. - or - *output* is the same stream we extract from. - OR - It is impossible to save archive in *cpioFormat* due to format restrictions. |

## Remarks

*output* must be writable.

## Examples

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(cpioFile);
    }
}       
```

### See Also

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


