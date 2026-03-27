---
title: CpioArchive.SaveLZMACompressed
second_title: Aspose.ZIP for .NET API Reference
description: CpioArchive method. Saves the archive to the stream with LZMA compression
type: docs
weight: 110
url: /net/aspose.zip.cpio/cpioarchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, CpioFormat) {#savelzmacompressed}

Saves the archive to the stream with LZMA compression.

```csharp
public void SaveLZMACompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Type | Description |
| --- | --- | --- |
| output | Stream | Destination stream. |
| cpioFormat | CpioFormat | Defines cpio header format. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | Archive has been disposed and cannot be used. |
| NotSupportedException | The stream does not support writing, or the stream is already closed. |

## Remarks

*output* must be writable.

Important: cpio archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

## Examples

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
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

## SaveLZMACompressed(string, CpioFormat) {#savelzmacompressed_1}

Saves the archive to the file by path with lzma compression.

```csharp
public void SaveLZMACompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| cpioFormat | CpioFormat | Defines cpio header format. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | Archive has been disposed and cannot be used. |
| ArgumentNullException | *path* is `null`. |
| Exception | Thrown when a runtime error occurs. |
| DirectoryNotFoundException | The specified path is invalid, (for example, it is on an unmapped drive). |
| IOException | An I/O error occurs. |
| PathTooLongException | The specified path, file name, or both exceed the system-defined maximum length. |
| UnauthorizedAccessException | The caller does not have the required permission. -or- *path* specified a read-only file or directory. |

## Remarks

Important: cpio archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

## Examples

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.cpio.lzma");
    }
}
```

### See Also

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


