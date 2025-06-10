---
title: CabArchive.CabArchive
second_title: Aspose.ZIP for .NET API Reference
description: CabArchive constructor. Initializes a new instance of the CabArchive class and composes an entry list can be extracted from the archive
type: docs
weight: 10
url: /net/aspose.zip.cab/cabarchive/cabarchive/
---
## CabArchive(Stream, CabLoadOptions) {#constructor}

Initializes a new instance of the [`CabArchive`](../) class and composes an entry list can be extracted from the archive.

```csharp
public CabArchive(Stream sourceStream, CabLoadOptions loadOptions = null)
```

| Parameter | Description |
| --- | --- |
| sourceStream | The source of the archive. It must be seekable. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceStream* is null. |
| ArgumentException | *sourceStream* is not seekable. |
| InvalidDataException | *sourceStream* is not valid cab archive. |
| EndOfStreamException | The stream is too short. |

## Remarks

This constructor does not unpack any entry. See [`Open`](../../cabentry/open/) method for unpacking.

## Examples

The following example shows how to extract all the entries to a directory.

```csharp
using (var archive = new CabArchive(File.OpenRead("archive.cab")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### See Also

* class [CabLoadOptions](../../cabloadoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CabArchive(string, CabLoadOptions) {#constructor_1}

Initializes a new instance of the [`CabArchive`](../) class and composes an entry list can be extracted from the archive.

```csharp
public CabArchive(string path, CabLoadOptions loadOptions = null)
```

| Parameter | Description |
| --- | --- |
| path | The path to the archive file. |

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
| EndOfStreamException | The file is too short. |

## Remarks

This constructor does not unpack any entry. See [`Open`](../../cabentry/open/) method for unpacking.

## Examples

The following example shows how to extract all the entries to a directory.

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### See Also

* class [CabLoadOptions](../../cabloadoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


