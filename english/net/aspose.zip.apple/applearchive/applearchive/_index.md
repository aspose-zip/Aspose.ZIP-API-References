---
title: AppleArchive.AppleArchive
second_title: Aspose.ZIP for .NET API Reference
description: AppleArchive constructor. Initializes a new instance of the AppleArchive class with settings used for composed entries
type: docs
weight: 10
url: /net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

Initializes a new instance of the [`AppleArchive`](../) class with settings used for composed entries.

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | Settings used when composing a new Apple Archive. |

### See Also

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

Initializes a new instance of the [`AppleArchive`](../) class and composes an entry list can be extracted from the archive.

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | The source of the archive. |
| loadOptions | AppleArchiveLoadOptions | Options to load existing archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceStream* is null. |
| ArgumentException | *sourceStream* is not seekable. |
| InvalidDataException | *sourceStream* is not a valid Apple Archive. |
| EndOfStreamException | The stream ends unexpectedly during parsing of the archive entries. |

## Remarks

This constructor does not decompress any entry. See [`ExtractToDirectory`](../extracttodirectory/) and [`Open`](../../applearchiveentry/open/) methods for decompressing.

### See Also

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

Initializes a new instance of the [`AppleArchive`](../) class and composes an entry list can be extracted from the archive.

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The fully qualified or the relative path to the archive file. |
| loadOptions | AppleArchiveLoadOptions | Options to load existing archive with. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* is null. |
| FileNotFoundException | The file is not found. |
| InvalidDataException | *path* is not a valid Apple Archive. |
| EndOfStreamException | The stream ends unexpectedly during parsing of the archive entries. |

## Remarks

This constructor does not decompress any entry. See [`ExtractToDirectory`](../extracttodirectory/) and [`Open`](../../applearchiveentry/open/) methods for decompressing.

### See Also

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


