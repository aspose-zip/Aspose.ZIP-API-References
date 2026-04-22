---
title: AppleArchive.Save
second_title: Aspose.ZIP for .NET API Reference
description: AppleArchive method. Saves archive to the stream provided
type: docs
weight: 70
url: /net/aspose.zip.apple/applearchive/save/
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
| ObjectDisposedException | The archive has been disposed. |
| ArgumentNullException | *output* is `null`. |
| ArgumentException | *output* is not writable. |
| ArgumentOutOfRangeException | Configured LZ4 block size is not positive. |
| NotSupportedException | Compression settings are missing or unsupported, direct composition uses a non-seekable stream, or entry/archive size exceeds current Apple Archive limits. |

## Remarks

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### See Also

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Saves archive to a destination file provided.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | String | The path of the archive to be created. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | The archive has been disposed. |
| ArgumentException | *destinationFileName* is invalid. |
| ArgumentNullException | *destinationFileName* is `null`. |
| ArgumentOutOfRangeException | Configured LZ4 block size is not positive. |
| NotSupportedException | Compression settings are missing or unsupported, direct composition uses a non-seekable stream, or entry/archive size exceeds current Apple Archive limits. |

### See Also

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


