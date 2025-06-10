---
title: XarArchive.XarArchive
second_title: Aspose.ZIP for .NET API Reference
description: XarArchive constructor. Initializes a new instance of the XarArchive class
type: docs
weight: 10
url: /net/aspose.zip.xar/xararchive/xararchive/
---
## XarArchive(XarCompressionSettings) {#constructor}

Initializes a new instance of the [`XarArchive`](../) class.

```csharp
public XarArchive(XarCompressionSettings defaultCompressionSettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| defaultCompressionSettings | XarCompressionSettings | The default compression settings, applyed to all entries of the archive. |

## Examples

The following example shows how to compress a file.

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### See Also

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## XarArchive(Stream, XarLoadOptions) {#constructor_1}

Initializes a new instance of the [`XarArchive`](../) class and composes an entry list can be extracted from the archive.

```csharp
public XarArchive(Stream sourceStream, XarLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | The source of the archive. It must be seekable. |
| loadOptions | XarLoadOptions | The options to load archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceStream* is null. |
| ArgumentException | *sourceStream* is not seekable. |
| InvalidDataException | *sourceStream* is not valid xar archive. |

## Remarks

This constructor does not unpack any entry. See [`Open`](../../xarfileentry/open/) method for unpacking.

## Examples

The following example shows how to extract all the entries to a directory.

```csharp
using (var archive = new XarArchive(File.OpenRead("archive.xar")))
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### See Also

* class [XarLoadOptions](../../xarloadoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## XarArchive(string, XarLoadOptions) {#constructor_2}

Initializes a new instance of the [`XarArchive`](../) class and composes an entry list can be extracted from the archive.

```csharp
public XarArchive(string path, XarLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the archive file. |
| loadOptions | XarLoadOptions | The options to load archive with. |

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
| InvalidDataException | File at *path* is not valid xar archive. |

## Remarks

This constructor does not unpack any entry. See [`Open`](../../xarfileentry/open/) method for unpacking.

## Examples

The following example shows how to extract all the entries to a directory.

```csharp
using (var archive = new XarArchive("archive.xar")) 
{
   archive.ExtractToDirectory("C:\\extracted");
}
```

### See Also

* class [XarLoadOptions](../../xarloadoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


