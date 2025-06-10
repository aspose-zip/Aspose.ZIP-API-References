---
title: WimArchive.WimArchive
second_title: Aspose.ZIP for .NET API Reference
description: WimArchive constructor. Initializes a new instance of the WimArchive class and composes an entry list can be extracted from the archive
type: docs
weight: 10
url: /net/aspose.zip.wim/wimarchive/wimarchive/
---
## WimArchive(Stream, WimLoadOptions) {#constructor}

Initializes a new instance of the [`WimArchive`](../) class and composes an entry list can be extracted from the archive.

```csharp
public WimArchive(Stream sourceStream, WimLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | The source of the archive. It must be seekable. |
| loadOptions | WimLoadOptions | Options to load existing archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceStream* is null. |
| ArgumentException | *sourceStream* is not seekable. |
| InvalidDataException | *sourceStream* is not valid wim archive. |

## Remarks

This constructor does not unpack any entry. See [`Open`](../../wimfileentry/open/) method for unpacking.

## Examples

The following example shows how to extract all the entries to a directory.

```csharp
using (var archive = new WimArchive(File.OpenRead("archive.wim")))
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### See Also

* class [WimLoadOptions](../../wimloadoptions/)
* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)

---

## WimArchive(string, WimLoadOptions) {#constructor_1}

Initializes a new instance of the [`WimArchive`](../) class and composes an entry list can be extracted from the archive.

```csharp
public WimArchive(string path, WimLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the archive file. |
| loadOptions | WimLoadOptions | Options to load existing archive with. |

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

This constructor does not unpack any entry. See [`Open`](../../wimfileentry/open/) method for unpacking.

## Examples

The following example shows how to extract all the entries to a directory.

```csharp
using (var archive = new WimArchive("archive.wim")) 
{ 
   archive.Images[0].ExtractToDirectory("C:\\extracted");
}
```

### See Also

* class [WimLoadOptions](../../wimloadoptions/)
* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)


