---
title: Lz4Archive.Lz4Archive
second_title: Aspose.ZIP for .NET API Reference
description: Lz4Archive constructor. Initializes a new instance of the Lz4Archive class prepared for decompressing
type: docs
weight: 10
url: /net/aspose.zip.lz4/lz4archive/lz4archive/
---
## Lz4Archive(Stream, Lz4LoadOptions) {#constructor_1}

Initializes a new instance of the [`Lz4Archive`](../) class prepared for decompressing.

```csharp
public Lz4Archive(Stream sourceStream, Lz4LoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | The source of the archive. |
| loadOptions | Lz4LoadOptions | The options to load archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Cannot read from *sourceStream* |
| ArgumentNullException | *sourceStream* is null. |
| EndOfStreamException | *sourceStream* is too short. |
| InvalidDataException | The *sourceStream* has wrong signature. |

## Remarks

This constructor does not decompress. See [`Open`](../open/) method for decompressing.

## Examples

Open an archive from a stream and extract it to a `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive(File.OpenRead("archive.lz4")))
  archive.Open().CopyTo(ms);
```

### See Also

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(string, Lz4LoadOptions) {#constructor_2}

Initializes a new instance of the [`Lz4Archive`](../) class.

```csharp
public Lz4Archive(string path, Lz4LoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the archive file. |
| loadOptions | Lz4LoadOptions | The options to load archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | The caller does not have the required permission to access |
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* contains a colon (:) in the middle of the string. |
| EndOfStreamException | The file is too short. |
| InvalidDataException | Data in the file has the wrong signature. |

## Remarks

This constructor does not decompress. See [`Open`](../open/) method for decompressing.

## Examples

Open an archive from file by path and extract it to a `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive("archive.lz4"))
  archive.Open().CopyTo(ms);
```

### See Also

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(Lz4ArchiveSetting) {#constructor}

Initializes a new instance of the [`Lz4Archive`](../) class prepared for compressing.

```csharp
public Lz4Archive(Lz4ArchiveSetting settings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| settings | Lz4ArchiveSetting | The setting of the composed archive. |

### See Also

* class [Lz4ArchiveSetting](../../lz4archivesetting/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


