---
title: UueArchive.UueArchive
second_title: Aspose.ZIP for .NET API Reference
description: UueArchive constructor. Initializes a new instance of the UueArchive class prepared for encoding
type: docs
weight: 10
url: /net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

Initializes a new instance of the [`UueArchive`](../) class prepared for encoding.

```csharp
public UueArchive()
```

## Examples

The following example shows how to uuencode file.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### See Also

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

Initializes a new instance of the [`UueArchive`](../) class prepared for decoding.

```csharp
public UueArchive(Stream sourceStream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | The source of the archive. |

## Remarks

This constructor does not decode. See [`Open`](../open/) method for decompressing.

## Examples

Open an archive from a stream and extract it to a `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### See Also

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

Initializes a new instance of the [`UueArchive`](../) class.

```csharp
public UueArchive(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the archive file. |

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

Open an archive from file by path and decode it to a `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### See Also

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


