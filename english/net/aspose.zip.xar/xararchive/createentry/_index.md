---
title: XarArchive.CreateEntry
second_title: Aspose.ZIP for .NET API Reference
description: XarArchive method. Create a single entry within the archive
type: docs
weight: 40
url: /net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

Create a single entry within the archive.

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| fileInfo | FileInfo | The metadata of file or folder to be compressed. |
| openImmediately | Boolean | True, if open the file immediately, otherwise open the file on archive saving. |
| compressionSettings | XarCompressionSettings | The compression settings used for added [`XarEntry`](../../xarentry/) item. |

### Return Value

Xar entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *name* is null. |
| ArgumentException | *name* is empty. |
| ArgumentNullException | *fileInfo* is null. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Remarks

If the file is opened immediately with *openImmediately* parameter it becomes blocked until archive is disposed.

## Examples

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### See Also

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

Create a single entry within the archive.

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| sourcePath | String | Path to file to be compressed. |
| openImmediately | Boolean | True, if open the file immediately, otherwise open the file on archive saving. |
| compressionSettings | XarCompressionSettings | The compression settings used for added [`XarEntry`](../../xarentry/) item. |

### Return Value

Xar entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourcePath* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *sourcePath* is empty, contains only white spaces, or contains invalid characters. - or - File name, as a part of *name*, exceeds 100 symbols. |
| UnauthorizedAccessException | Access to file *sourcePath* is denied. |
| PathTooLongException | The specified *sourcePath*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. - or - *name* is too long for xar. |
| NotSupportedException | File at *sourcePath* contains a colon (:) in the middle of the string. |
| InvalidOperationException | Impossible to modify xar archive. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Remarks

The entry name is solely set within *name* parameter. The file name provided in *sourcePath* parameter does not affect the entry name.

If the file is opened immediately with *openImmediately* parameter it becomes blocked until archive is disposed.

## Examples

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### See Also

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

Create a single entry within the archive.

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| source | Stream | The input stream for the entry. |
| compressionSettings | XarCompressionSettings | The compression settings used for added [`XarEntry`](../../xarentry/) item. |

### Return Value

Xar entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *name* is null. |
| ArgumentNullException | *source* is null. |
| ArgumentException | *name* is empty. |
| InvalidOperationException | Impossible to modify xar archive. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Examples

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### See Also

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


