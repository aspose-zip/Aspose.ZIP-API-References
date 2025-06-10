---
title: SharArchive.CreateEntries
second_title: Aspose.ZIP for .NET API Reference
description: SharArchive method. Adds to the archive all the files and directories recursively in the directory given
type: docs
weight: 30
url: /net/aspose.zip.shar/shararchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Adds to the archive all the files and directories recursively in the directory given.

```csharp
public SharArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | String | Directory to compress. |
| includeRootDirectory | Boolean | Indicates whether to include the root directory itself or not. |

### Return Value

Shar entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceDirectory* is null. |
| SecurityException | The caller does not have the required permission to access *sourceDirectory*. |
| ArgumentException | *sourceDirectory* contains invalid characters such as ", &lt;, &gt;, or &#x7C;. |
| PathTooLongException | The specified path, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. The specified path, file name, or both are too long. |
| IOException | *sourceDirectory* stands for a file, not for a directory. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Examples

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(sharFile);
    }
}
```

### See Also

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Adds to the archive all the files and directories recursively in the directory given.

```csharp
public SharArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Type | Description |
| --- | --- | --- |
| directory | DirectoryInfo | Directory to compress. |
| includeRootDirectory | Boolean | Indicates whether to include the root directory itself or not. |

### Return Value

Shar entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *directory* is null. |
| SecurityException | The caller does not have the required permission to access *directory*. |
| IOException | *directory* stands for a file, not for a directory. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Examples

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(sharFile);
    }
}
```

### See Also

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


