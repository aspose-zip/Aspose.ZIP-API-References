---
title: TarArchive.SaveXzCompressed
second_title: Aspose.ZIP for .NET API Reference
description: TarArchive method. Saves archive to the stream with xz compression
type: docs
weight: 200
url: /net/aspose.zip.tar/tararchive/savexzcompressed/
---
## SaveXzCompressed(Stream, TarFormat?, XzArchiveSettings) {#savexzcompressed}

Saves archive to the stream with xz compression.

```csharp
public void SaveXzCompressed(Stream output, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| output | Stream | Destination stream. |
| format | Nullable`1 | Defines the tar header format. Null value will be treated as USTar when possible. |
| settings | XzArchiveSettings | Set of setting particular xz archive: dictionary size, block size, check type. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *output* is null. |
| ArgumentException | *output* is not writable. |

## Remarks

*output*The stream must be writable.

## Examples

```csharp
using (FileStream result = File.OpenWrite("result.tar.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### See Also

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, TarFormat?, XzArchiveSettings) {#savexzcompressed_1}

Saves archive to the path by path with xz compression.

```csharp
public void SaveXzCompressed(string path, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| format | Nullable`1 | Defines the tar header format. Null value will be treated as USTar when possible. |
| settings | XzArchiveSettings | Set of setting particular xz archive: dictionary size, block size, check type. |

### Exceptions

| exception | condition |
| --- | --- |
| UnauthorizedAccessException | The caller does not have the required permission. -or- *path* specified a read-only file or directory. |
| ArgumentException | *path* is a zero-length string, contains only white space, or contains one or more invalid characters as defined by InvalidPathChars. |
| ArgumentNullException | *path* is null. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| DirectoryNotFoundException | The specified *path* is invalid, (for example, it is on an unmapped drive). |
| NotSupportedException | *path* is in an invalid format. |

## Examples

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.tar.xz");
    }
}
```

### See Also

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


