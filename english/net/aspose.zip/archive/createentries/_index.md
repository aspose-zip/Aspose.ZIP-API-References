---
title: Archive.CreateEntries
second_title: Aspose.ZIP for .NET API Reference
description: Archive method. Adds to the archive all files and directories recursively in the directory given
type: docs
weight: 40
url: /net/aspose.zip/archive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Adds to the archive all files and directories recursively in the directory given.

```csharp
public Archive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Type | Description |
| --- | --- | --- |
| directory | DirectoryInfo | Directory to compress. |
| includeRootDirectory | Boolean | Indicates whether to include the root directory itself or not. |

### Return Value

The archive with entries composed.

### Exceptions

| exception | condition |
| --- | --- |
| DirectoryNotFoundException | The path to *directory* is invalid, such as being on an unmapped drive. |
| SecurityException | The caller does not have the required permission to access *directory*. |

## Examples

```csharp
using (Archive archive = new Archive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.zip");
}
```

### See Also

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Adds to the archive all files and directories recursively in the directory given.

```csharp
public Archive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | String | Directory to compress. |
| includeRootDirectory | Boolean | Indicates whether to include the root directory itself or not. |

### Return Value

The archive with entries composed.

## Examples

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.zip");
}
```

### See Also

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


