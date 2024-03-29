---
title: SaveLZMACompressed
second_title: Aspose.ZIP for .NET API Reference
description: 
type: docs
weight: 170
url: /net/aspose.zip.tar/tararchive/savelzmacompressed/
---
## TarArchive.SaveLZMACompressed method (1 of 2)

Saves archive to the stream with LZMA compression.

```csharp
public void SaveLZMACompressed(Stream output, TarFormat? format = default)
```

| Parameter | Type | Description |
| --- | --- | --- |
| output | Stream | Destination stream. |
| format | Nullable`1 | Defines tar header format. Null value will be treated as USTar when possible. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *output* is null. |
| ArgumentException | *output* is not writable. |

### Remarks

*output* must be writable.

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

### Examples

```csharp
using (FileStream result = File.OpenWrite("result.tar.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
        }
    }
}
```

### See Also

* enum [TarFormat](../../tarformat)
* class [TarArchive](../../tararchive)
* namespace [Aspose.Zip.Tar](../../tararchive)
* assembly [Aspose.Zip](../../../)

---

## TarArchive.SaveLZMACompressed method (2 of 2)

Saves archive to the file by path with lzma compression.

```csharp
public void SaveLZMACompressed(string path, TarFormat? format = default)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| format | Nullable`1 | Defines tar header format. Null value will be treated as USTar when possible. |

### Remarks

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

### Examples

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.tar.lzma");
    }
}
```

### See Also

* enum [TarFormat](../../tarformat)
* class [TarArchive](../../tararchive)
* namespace [Aspose.Zip.Tar](../../tararchive)
* assembly [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.ZIP.dll -->