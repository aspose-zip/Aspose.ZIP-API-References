---
title: CreateEntries
second_title: Aspose.ZIP for .NET API Reference
description: 
type: docs
weight: 30
url: /net/aspose.zip.xar/xararchive/createentries/
---
## XarArchive.CreateEntries method (1 of 2)

Adds to the archive all the files and directories recursively in the directory given.

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | String | Directory to compress. |
| compressionSettings | Boolean | The compression settings used for added [`XarEntry`](../../xarentry) items. |
| includeRootDirectory | XarCompressionSettings | Indicates whether to include the root directory itself or not. |

### Return Value

Xar entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceDirectory* is null. |
| SecurityException | The caller does not have the required permission to access *sourceDirectory*. |
| ArgumentException | *sourceDirectory* contains invalid characters such as ", &lt;, &gt;, or &#x7C;. |
| PathTooLongException | The specified path, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. The specified path, file name, or both are too long. |
| IOException | *sourceDirectory* stands for a file, not for a directory. |

### Examples

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(@"C:\folder", false);
        archive.Save(xarFile);
    }
}
```

### See Also

* class [XarCompressionSettings](../../xarcompressionsettings)
* class [XarArchive](../../xararchive)
* namespace [Aspose.Zip.Xar](../../xararchive)
* assembly [Aspose.Zip](../../../)

---

## XarArchive.CreateEntries method (2 of 2)

Adds to the archive all the files and directories recursively in the directory given.

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| directory | DirectoryInfo | Directory to compress. |
| compressionSettings | Boolean | The compression settings used for added [`XarEntry`](../../xarentry) items. |
| includeRootDirectory | XarCompressionSettings | Indicates whether to include the root directory itself or not. |

### Return Value

Xar entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *directory* is null. |
| SecurityException | The caller does not have the required permission to access *directory*. |
| IOException | *directory* stands for a file, not for a directory. |

### Examples

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(new DirectoryInfo(@"C:\folder"), false);
        archive.Save(xarFile);
    }
}
```

### See Also

* class [XarCompressionSettings](../../xarcompressionsettings)
* class [XarArchive](../../xararchive)
* namespace [Aspose.Zip.Xar](../../xararchive)
* assembly [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.ZIP.dll -->
