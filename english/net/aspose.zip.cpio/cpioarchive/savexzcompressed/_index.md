---
title: SaveXzCompressed
second_title: Aspose.ZIP for .NET API Reference
description: 
type: docs
weight: 100
url: /net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## CpioArchive.SaveXzCompressed method (1 of 2)

Saves archive to the stream with xz compression.

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| output | Stream | Destination stream. |
| cpioFormat | CpioFormat | Defines cpio header format. |
| settings | XzArchiveSettings | Set of setting particular xz archive: dictionary size, block size, check type. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *output* is null. |
| ArgumentException | *output* is not writable. |

### Remarks

*output*The stream must be writable.

### Examples

```csharp
using (FileStream result = File.OpenWrite("result.cpio.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### See Also

* enum [CpioFormat](../../cpioformat)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings)
* class [CpioArchive](../../cpioarchive)
* namespace [Aspose.Zip.Cpio](../../cpioarchive)
* assembly [Aspose.Zip](../../../)

---

## CpioArchive.SaveXzCompressed method (2 of 2)

Saves archive to the path by path with xz compression.

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| cpioFormat | CpioFormat | Defines cpio header format. |
| settings | XzArchiveSettings | Set of setting particular xz archive: dictionary size, block size, check type. |

### Examples

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.cpio.xz");
    }
}
```

### See Also

* enum [CpioFormat](../../cpioformat)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings)
* class [CpioArchive](../../cpioarchive)
* namespace [Aspose.Zip.Cpio](../../cpioarchive)
* assembly [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.ZIP.dll -->
