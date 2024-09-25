---
title: ZstandardArchive.ZstandardArchive
second_title: Aspose.ZIP for .NET API Reference
description: ZstandardArchive constructor. Initializes a new instance of the ZstandardArchive class prepared for compressing
type: docs
weight: 10
url: /net/aspose.zip.zstandard/zstandardarchive/zstandardarchive/
---
## ZstandardArchive() {#constructor}

Initializes a new instance of the [`ZstandardArchive`](../) class prepared for compressing.

```csharp
public ZstandardArchive()
```

## Examples

The following example shows how to compress a file.

```csharp
using (ZstandardArchive archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### See Also

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(Stream, ZstandardLoadOptions) {#constructor_1}

Initializes a new instance of the [`ZstandardArchive`](../) class prepared for decompressing.

```csharp
public ZstandardArchive(Stream sourceStream, ZstandardLoadOptions options = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | The source of the archive. |
| options | ZstandardLoadOptions | The options to load archive with. |

## Remarks

This constructor does not decompress. See [`Open`](../open/) method for decompressing.

## Examples

Open an archive from a stream and extract it to a `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new ZstandardArchive(File.OpenRead("archive.zst")))
  archive.Open().CopyTo(ms);
```

### See Also

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(string, ZstandardLoadOptions) {#constructor_2}

Initializes a new instance of the [`ZstandardArchive`](../) class.

```csharp
public ZstandardArchive(string path, ZstandardLoadOptions options = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the archive file. |
| options | ZstandardLoadOptions | The options to load archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* contains a colon (:) in the middle of the string. |

## Remarks

This constructor does not decompress. See [`Open`](../open/) method for decompressing.

## Examples

Open an archive from file by path and extract it to a `MemoryStream`

```csharp
var ms = new MemoryStream();
using (ZstandardArchive archive = new ZstandardArchive("archive.zst"))
  archive.Open().CopyTo(ms);
```

### See Also

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


