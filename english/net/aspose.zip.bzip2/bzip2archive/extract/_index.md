---
title: Bzip2Archive.Extract
second_title: Aspose.ZIP for .NET API Reference
description: Bzip2Archive method. Extracts the archive to the stream provided
type: docs
weight: 30
url: /net/aspose.zip.bzip2/bzip2archive/extract/
---
## Extract(Stream) {#extract_1}

Extracts the archive to the stream provided.

```csharp
public void Extract(Stream destination)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destination | Stream | Destination stream. Must be writable. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *destination* does not support writing. |

## Examples

```csharp
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
{
     archive.Extract(httpResponseStream);
}
```

### See Also

* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Extracts the archive to the file by path.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to destination file. If the file already exists, it will be overwritten. |

### Return Value

Info of extracted file.

### See Also

* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


