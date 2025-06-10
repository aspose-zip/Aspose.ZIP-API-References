---
title: CpioArchive.CreateEntries
second_title: Aspose.ZIP for .NET API Reference
description: CpioArchive method. Adds to the archive all the files and directories recursively in the directory given
type: docs
weight: 30
url: /net/aspose.zip.cpio/cpioarchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Adds to the archive all the files and directories recursively in the directory given.

```csharp
public CpioArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | String | Directory to compress. |
| includeRootDirectory | Boolean | Indicates whether to include the root directory itself or not. |

### Return Value

Cpio entry instance.

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
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(cpioFile);
    }
}
```

### See Also

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Adds to the archive all the files and directories recursively in the directory given.

```csharp
public CpioArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Type | Description |
| --- | --- | --- |
| directory | DirectoryInfo | Directory to compress. |
| includeRootDirectory | Boolean | Indicates whether to include the root directory itself or not. |

### Return Value

Cpio entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *directory* is null. |
| SecurityException | The caller does not have the required permission to access *directory*. |
| IOException | *directory* stands for a file, not for a directory. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Examples

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(cpioFile);
    }
}
```

### See Also

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


