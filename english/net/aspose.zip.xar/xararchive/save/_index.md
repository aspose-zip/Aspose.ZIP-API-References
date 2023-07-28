---
title: XarArchive.Save
second_title: Aspose.ZIP for .NET API Reference
description: XarArchive method. Saves archive to destination file provided
type: docs
weight: 80
url: /net/aspose.zip.xar/xararchive/save/
---
## Save(string) {#save_1}

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

* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream) {#save}

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

* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


