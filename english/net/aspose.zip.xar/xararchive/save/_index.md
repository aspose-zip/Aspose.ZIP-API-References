---
title: Save
second_title: Aspose.ZIP for .NET API Reference
description: 
type: docs
weight: 80
url: /net/aspose.zip.xar/xararchive/save/
---
## XarArchive.Save method (1 of 2)

Saves archive to destination file provided.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationFileName* is null. |
| InvalidOperationException | Impossible to modify xar archive. |

### See Also

* class [XarArchive](../../xararchive)
* namespace [Aspose.Zip.Xar](../../xararchive)
* assembly [Aspose.Zip](../../../)

---

## XarArchive.Save method (2 of 2)

Saves archive to the stream provided.

```csharp
public void Save(Stream output)
```

| Parameter | Type | Description |
| --- | --- | --- |
| output | Stream | Destination stream. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *output* is null. |
| ArgumentException | *output*Is not writable/readable or not seekable. |
| InvalidOperationException | Impossible to modify xar archive. |

### See Also

* class [XarArchive](../../xararchive)
* namespace [Aspose.Zip.Xar](../../xararchive)
* assembly [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.ZIP.dll -->