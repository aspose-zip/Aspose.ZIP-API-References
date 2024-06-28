---
title: TarArchive.TarArchive
second_title: Aspose.ZIP for .NET API Reference
description: TarArchive constructor. Initializes a new instance of the TarArchive class
type: docs
weight: 10
url: /net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

Initializes a new instance of the [`TarArchive`](../) class.

```csharp
public TarArchive()
```

## Examples

The following example shows how to compress a file.

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## TarArchive(Stream) {#constructor_1}

Initializes a new instance of the [`Archive`](../../../aspose.zip/archive/) class and composes entries list can be extracted from the archive.

```csharp
public TarArchive(Stream sourceStream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | The source of the archive. It must be seekable. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidDataException | *sourceStream* is not seekable. |

## Remarks

This constructor does not unpack any entry. See [`Open`](../../tarentry/open/) method for unpacking.

## Examples

The following example shows how to extract all of the entries to a directory.

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## TarArchive(string) {#constructor_2}

Initializes a new instance of the [`TarArchive`](../) class and composes entries list can be extracted from the archive.

```csharp
public TarArchive(string path)
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
| FileNotFoundException | The file is not found. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| IOException | The file is already open. |

## Remarks

This constructor does not unpack any entry. See [`Open`](../../tarentry/open/) method for unpacking.

## Examples

The following example shows how to extract all of the entries to a directory.

```csharp
using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


