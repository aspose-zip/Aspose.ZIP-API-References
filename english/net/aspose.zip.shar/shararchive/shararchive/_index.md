---
title: SharArchive.SharArchive
second_title: Aspose.ZIP for .NET API Reference
description: SharArchive constructor. Initializes a new instance of the SharArchive class
type: docs
weight: 10
url: /net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

Initializes a new instance of the [`SharArchive`](../) class.

```csharp
public SharArchive()
```

## Examples

The following example shows how to compress a file.

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### See Also

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

Initializes a new instance of the [`SharArchive`](../) class prepared for decompressing.

```csharp
public SharArchive(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | Path to the source of the archive. |

### See Also

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


