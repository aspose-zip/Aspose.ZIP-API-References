---
title: CpioArchive.SaveZstandard
second_title: Aspose.ZIP for .NET API Reference
description: CpioArchive method. Saves archive to the stream with Zstandard compression
type: docs
weight: 140
url: /net/aspose.zip.cpio/cpioarchive/savezstandard/
---
## SaveZstandard(Stream, CpioFormat) {#savezstandard}

Saves archive to the stream with Zstandard compression.

```csharp
public void SaveZstandard(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
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

## Remarks

*output* must be writable.

## Examples

```csharp
using (FileStream result = File.OpenWrite("result.cpio.zst"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZstandard(result);
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

## SaveZstandard(string, CpioFormat) {#savezstandard_1}

Saves archive to the file by path with Zstandard compression.

```csharp
public void SaveZstandard(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| cpioFormat | CpioFormat | Defines cpio header format. |

## Examples

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZstandard("result.cpio.zst");
    }
}
```

### See Also

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


