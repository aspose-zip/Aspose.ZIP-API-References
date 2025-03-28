---
title: Bzip2Archive.Bzip2Archive
second_title: Aspose.ZIP for .NET API Reference
description: Bzip2Archive constructor. Initializes a new instance of the Bzip2Archive class prepared for compressing
type: docs
weight: 10
url: /net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

Initializes a new instance of the [`Bzip2Archive`](../) class prepared for compressing.

```csharp
public Bzip2Archive()
```

## Examples

The following example shows how to compress a file.

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### See Also

* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream, Bzip2LoadOptions) {#constructor_1}

Initializes a new instance of the [`Bzip2Archive`](../) class prepared for decompressing.

```csharp
public Bzip2Archive(Stream sourceStream, Bzip2LoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | The source of the archive. |
| loadOptions | Bzip2LoadOptions | The options to load archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| EndOfStreamException | Premature stream end. |
| InvalidDataException | Wrong signature bytes. |

## Remarks

This constructor does not decompress. See [`Open`](../open/) method for decompressing.

## Examples

Open an archive from a stream and extract it to a `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### See Also

* class [Bzip2LoadOptions](../../bzip2loadoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2Archive(string, Bzip2LoadOptions) {#constructor_2}

Initializes a new instance of the [`Bzip2Archive`](../) class prepared for decompressing.

```csharp
public Bzip2Archive(string path, Bzip2LoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the archive file. |
| loadOptions | Bzip2LoadOptions | The options to load archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* contains a colon (:) in the middle of the string. |
| FileNotFoundException | The file is not found. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| IOException | The file is already open. |
| EndOfStreamException | Premature stream end. |
| InvalidDataException | Wrong signature bytes. |

## Remarks

This constructor does not decompress. See [`Open`](../open/) method for decompressing.

## Examples

Open an archive from file by path and extract it to a `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### See Also

* class [Bzip2LoadOptions](../../bzip2loadoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


