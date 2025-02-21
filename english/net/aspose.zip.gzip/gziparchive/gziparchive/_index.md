---
title: GzipArchive.GzipArchive
second_title: Aspose.ZIP for .NET API Reference
description: GzipArchive constructor. Initializes a new instance of the GzipArchive class prepared for compressing
type: docs
weight: 10
url: /net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

Initializes a new instance of the [`GzipArchive`](../) class prepared for compressing.

```csharp
public GzipArchive()
```

## Examples

The following example shows how to compress a file.

```csharp
using (GzipArchive archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### See Also

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(Stream, bool) {#constructor_1}

Initializes a new instance of the [`GzipArchive`](../) class prepared for decompressing.

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | The source of the archive. |
| parseHeader | Boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceStream* is null. |
| EndOfStreamException | *sourceStream* is too short. |
| InvalidDataException | The *sourceStream* has wrong signature. |

## Remarks

This constructor does not decompress. See [`Open`](../open/) method for decompressing.

## Examples

Open an archive from a stream and extract it to a `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### See Also

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_2}

Initializes a new instance of the [`GzipArchive`](../) class.

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the archive file. |
| parseHeader | Boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* contains a colon (:) in the middle of the string. |
| EndOfStreamException | File is too short. |
| InvalidDataException | Data in the file has wrong signature. |

## Remarks

This constructor does not decompress. See [`Open`](../open/) method for decompressing.

## Examples

Open an archive from file by path and extract it to a `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### See Also

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


