---
title: IsoArchive.IsoArchive
second_title: Aspose.ZIP for .NET API Reference
description: IsoArchive constructor. Initializes a new instance of the IsoArchive class and creates an empty ISO archive for adding new files and directories
type: docs
weight: 10
url: /net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

Initializes a new instance of the [`IsoArchive`](../) class and creates an empty ISO archive for adding new files and directories.

```csharp
public IsoArchive()
```

## Examples

The following example shows how to create a new empty ISO archive and add files to it:

```csharp
// Create a new empty ISO archive
using(IsoArchive isoArchive = new IsoArchive())
{
    // Add files to the ISO archive
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Save the ISO archive to a file
    isoArchive.Save("new_archive.iso");
}
```

### See Also

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

Initializes a new instance of the [`IsoArchive`](../) class and composes an entry list that can be extracted from the archive.

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | The source of the archive. It must be seekable. |
| loadOptions | IsoLoadOptions | The options to load archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceStream* is null. |
| ArgumentException | *sourceStream* is not seekable. |
| InvalidDataException | *sourceStream* is not a valid ISO archive. |

## Remarks

This constructor does not unpack any entry.

## Examples

The following example shows how to extract all of the entries to a directory.

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### See Also

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

Initializes a new instance of the [`IsoArchive`](../) class and composes an entry list that can be extracted from the archive.

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the archive file. |
| loadOptions | IsoLoadOptions | The options to load archive with. |

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

This constructor does not unpack any entry.

## Examples

The following example shows how to extract all of the entries to a directory.

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### See Also

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


