---
title: CabArchive.CreateEntries
second_title: Aspose.ZIP for .NET API Reference
description: CabArchive method. Adds to the archive all files recursively from the specified directory
type: docs
weight: 30
url: /net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Adds to the archive all files, recursively, from the specified directory.

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Type | Description |
| --- | --- | --- |
| directory | DirectoryInfo | Directory to compress. |
| includeRootDirectory | Boolean | Indicates whether to include the root directory name in entry paths. |

### Return Value

The current [`CabArchive`](../) instance.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *directory* is null. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |
| DirectoryNotFoundException | *directory* cannot be found. |
| SecurityException | The caller does not have the required permission to access *directory* or its content. |
| UnauthorizedAccessException | Access to *directory* or one of its files is denied. |
| IOException | An I/O error occurs while accessing *directory*. |
| PathTooLongException | A generated entry path exceeds the system-defined maximum length. |
| InvalidOperationException | The archive is prepared for extraction and cannot add entries. |

## Examples

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### See Also

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Adds to the archive all files recursively from the specified directory path.

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | String | Directory path to compress. |
| includeRootDirectory | Boolean | Indicates whether to include the root directory name in entry paths. |

### Return Value

The current [`CabArchive`](../) instance.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | Archive has been disposed and cannot be used. |
| ArgumentNullException | *sourceDirectory* is null. |
| DirectoryNotFoundException | *sourceDirectory* cannot be found. |
| SecurityException | The caller does not have the required permission to access *sourceDirectory*. |
| UnauthorizedAccessException | Access to *sourceDirectory* is denied. |
| PathTooLongException | The specified *sourceDirectory* exceeds the system-defined maximum length. |
| ArgumentException | *sourceDirectory* is empty, contains only white spaces, or contains invalid characters. |
| IOException | An I/O error occurs while accessing *sourceDirectory*. |
| InvalidOperationException | The archive is prepared for extraction and cannot add entries. |

## Examples

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### See Also

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


