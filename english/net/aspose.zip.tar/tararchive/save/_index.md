---
title: TarArchive.Save
second_title: Aspose.ZIP for .NET API Reference
description: TarArchive method. Saves archive to the stream provided
type: docs
weight: 140
url: /net/aspose.zip.tar/tararchive/save/
---
## Save(Stream, TarFormat?) {#save}

Saves archive to the stream provided.

```csharp
public void Save(Stream output, TarFormat? format = default)
```

| Parameter | Type | Description |
| --- | --- | --- |
| output | Stream | Destination stream. |
| format | Nullable`1 | Defines tar header format. Null value will be treated as USTar when possible. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *output* is not writable. - or - *output* is the same stream we extract from. - OR - It is impossible to save archive in *format* due to format restrictions. |

## Remarks

*output* must be writable.

## Examples

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry1", "data.bin");
        archive.Save(tarFile);
    }
}       
```

### See Also

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, TarFormat?) {#save_1}

Saves archive to a destination file provided.

```csharp
public void Save(string destinationFileName, TarFormat? format = default)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| format | Nullable`1 | Defines the tar header format. Null value will be treated as USTar when possible. |

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

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file.

## Examples

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("myarchive.tar");
}       
```

### See Also

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


