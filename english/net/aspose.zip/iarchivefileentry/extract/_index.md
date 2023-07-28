---
title: IArchiveFileEntry.Extract
second_title: Aspose.ZIP for .NET API Reference
description: IArchiveFileEntry method. Extracts the entry to the filesystem by the path provided
type: docs
weight: 30
url: /net/aspose.zip/iarchivefileentry/extract/
---
## Extract(string) {#extract}

Extracts the entry to the filesystem by the path provided.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to destination file. If the file already exists, it will be overwritten. |

### Return Value

FileInfo instance containing extracted data.

### See Also

* interface [IArchiveFileEntry](../)
* namespace [Aspose.Zip](../../iarchivefileentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extracts the entry to the stream provided.

```csharp
public void Extract(Stream destination)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destination | Stream | Destination stream. Must be writable. |

### See Also

* interface [IArchiveFileEntry](../)
* namespace [Aspose.Zip](../../iarchivefileentry/)
* assembly [Aspose.Zip](../../../)


