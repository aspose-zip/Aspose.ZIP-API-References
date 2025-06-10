---
title: CpioArchive.SaveGzipped
second_title: Aspose.ZIP for .NET API Reference
description: CpioArchive method. Saves archive to the stream with gzip compression
type: docs
weight: 90
url: /net/aspose.zip.cpio/cpioarchive/savegzipped/
---
## SaveGzipped(Stream, CpioFormat) {#savegzipped}

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
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Remarks

*output* must be writable.

## Examples

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

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveGzipped(string, CpioFormat) {#savegzipped_1}

Saves archive to the file by path with gzip compression.

```csharp
public void SaveGzipped(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| cpioFormat | CpioFormat | Defines cpio header format. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Examples

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

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


