---
title: AlzArchive.AlzArchive
second_title: Aspose.ZIP for .NET API Reference
description: AlzArchive constructor. Initializes a new instance of the AlzArchive class from a stream
type: docs
weight: 10
url: /net/aspose.zip.alz/alzarchive/alzarchive/
---
## AlzArchive(Stream, AlzArchiveLoadOptions) {#constructor}

Initializes a new instance of the [`AlzArchive`](../) class from a stream.

```csharp
public AlzArchive(Stream stream, AlzArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The ALZ archive stream. The stream must support reading and seeking. |
| loadOptions | AlzArchiveLoadOptions | Options to load existing archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | stream is null. |

### See Also

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)

---

## AlzArchive(string, AlzArchiveLoadOptions) {#constructor_1}

Initializes a new instance of the [`AlzArchive`](../) class from a file path.

```csharp
public AlzArchive(string filePath, AlzArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | Path to the ALZ archive file. |
| loadOptions | AlzArchiveLoadOptions | Options to load existing archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | filePath is null. |
| FileNotFoundException | The file does not exist. |

### See Also

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)


