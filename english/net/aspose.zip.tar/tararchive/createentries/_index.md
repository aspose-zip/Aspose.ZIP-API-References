---
title: TarArchive.CreateEntries
second_title: Aspose.ZIP for .NET API Reference
description: TarArchive method. Adds to the archive all the files and directories recursively in the directory given
type: docs
weight: 70
url: /net/aspose.zip.tar/tararchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Adds to the archive all the files and directories recursively in the directory given.

```csharp
public TarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Type | Description |
| --- | --- | --- |
| directory | DirectoryInfo | Directory to compress. |
| includeRootDirectory | Boolean | Indicates whether to include the root directory itself or not. |

### Return Value

The archive with entries composed.

## Examples

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(tarFile);
    }
}
```

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Adds to the archive all the files and directories recursively in the directory given.

```csharp
public TarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | String | Directory to compress. |
| includeRootDirectory | Boolean | Indicates whether to include the root directory itself or not. |

### Return Value

The archive with entries composed.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceDirectory* is null. |
| SecurityException | The caller does not have the required permission to access *sourceDirectory*. |
| ArgumentException | *sourceDirectory* contains invalid characters such as ", &lt;, &gt;, or &#x7C;. |
| PathTooLongException | The specified path, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. The specified path, file name, or both are too long. |

## Examples

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(tarFile);
    }
}
```

### See Also

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


