---
title: SaveGzipped
second_title: Aspose.ZIP for .NET API Reference
description: 
type: docs
weight: 90
url: /net/aspose.zip.cpio/cpioarchive/savegzipped/
---
## CpioArchive.SaveGzipped method (1 of 2)

Saves archive to the stream with gzip compression.

```csharp
public void SaveGzipped(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Type | Description |
| --- | --- | --- |
| output | Stream | Destination stream. |
| cpioFormat | CpioFormat | Defines cpio header format. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *output* is null. |
| ArgumentException | *output* is not writable. |

### Remarks

*output* must be writable.

### Examples

```csharp
using (FileStream result = File.OpenWrite("result.cpio.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### See Also

* enum [CpioFormat](../../cpioformat)
* class [CpioArchive](../../cpioarchive)
* namespace [Aspose.Zip.Cpio](../../cpioarchive)
* assembly [Aspose.Zip](../../../)

---

## CpioArchive.SaveGzipped method (2 of 2)

Saves archive to the file by path with gzip compression.

```csharp
public void SaveGzipped(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| cpioFormat | CpioFormat | Defines cpio header format. |

### Examples

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.cpio.gz");
    }
}
```

### See Also

* enum [CpioFormat](../../cpioformat)
* class [CpioArchive](../../cpioarchive)
* namespace [Aspose.Zip.Cpio](../../cpioarchive)
* assembly [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.ZIP.dll -->
