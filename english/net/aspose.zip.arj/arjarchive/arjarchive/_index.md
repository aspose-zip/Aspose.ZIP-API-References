---
title: ArjArchive.ArjArchive
second_title: Aspose.ZIP for .NET API Reference
description: ArjArchive constructor. Initializes a new instance of the ArjArchive class and composes entries list can be extracted from the archive
type: docs
weight: 10
url: /net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream) {#constructor}

Initializes a new instance of the [`ArjArchive`](../) class and composes entries list can be extracted from the archive.

```csharp
public ArjArchive(Stream extractionSource)
```

| Parameter | Type | Description |
| --- | --- | --- |
| extractionSource | Stream | The source of the archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *extractionSource* is null. |
| ArgumentException | &gt;*extractionSource* does not support seeking. |
| InvalidDataException | Wrong signature for archive. - or - The file is not an ARJ archive. |
| NotSupportedException | Archive is garbled. |

## Remarks

This constructor does not decompress any entry. See [`Extract`](../../arjentryplain/extract/) method for decompressing.

### See Also

* class [ArjArchive](../)
* namespace [Aspose.Zip.ARJ](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string) {#constructor_1}

Initializes a new instance of the [`ArjArchive`](../) class and composes entries list can be extracted from the archive.

```csharp
public ArjArchive(string path)
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

This constructor does not unpack any entry. See [`Extract`](../../arjentryplain/extract/) method for decompressing.

## Examples

The following example shows how to extract all of the entries to a directory.

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### See Also

* class [ArjArchive](../)
* namespace [Aspose.Zip.ARJ](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


