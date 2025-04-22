---
title: SnappyArchive.SnappyArchive
second_title: Aspose.ZIP for .NET API Reference
description: SnappyArchive constructor. Initializes a new instance of the SnappyArchive class prepared for compressing
type: docs
weight: 10
url: /net/aspose.zip.snappy/snappyarchive/snappyarchive/
---
## SnappyArchive() {#constructor}

Initializes a new instance of the [`SnappyArchive`](../) class prepared for compressing.

```csharp
public SnappyArchive()
```

## Examples

The following example shows how to compress a file.

```csharp
using (SnappyArchive archive = new SnappyArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.snappy");
}
```

### See Also

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## SnappyArchive(Stream) {#constructor_1}

Initializes a new instance of the [`SnappyArchive`](../) class prepared for decompressing.

```csharp
public SnappyArchive(Stream source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Stream | The source of the archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *source* is not seekable. |
| ArgumentNullException | *source* is null. |

## Remarks

This constructor does not decompress. See [`Extract`](../extract/) method for decompressing.

### See Also

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)

---

## SnappyArchive(string) {#constructor_2}

Initializes a new instance of the [`SnappyArchive`](../) class prepared for decompressing.

```csharp
public SnappyArchive(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | Path to the source of the archive. |

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

## Remarks

This constructor does not decompress. See [`Extract`](../extract/) method for decompressing.

## Examples

```csharp
using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
{
    using (var archive = new SnappyArchive(sourceSnappyFile))
    {
         archive.Extract(extractedFile);
    }
   }
```

### See Also

* class [SnappyArchive](../)
* namespace [Aspose.Zip.Snappy](../../snappyarchive/)
* assembly [Aspose.Zip](../../../)


