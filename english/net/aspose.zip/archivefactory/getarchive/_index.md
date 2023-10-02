---
title: ArchiveFactory.GetArchive
second_title: Aspose.ZIP for .NET API Reference
description: ArchiveFactory method. Detects the archive format and creates the appropriate IArchive object according to the type of archive specified by the given path
type: docs
weight: 10
url: /net/aspose.zip/archivefactory/getarchive/
---
## GetArchive(string) {#getarchive_1}

Detects the archive format and creates the appropriate [`IArchive`](../../iarchive/) object according to the type of archive specified by the given path.

```csharp
public static IArchive GetArchive(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the archive to be analyzed. |

### Return Value

An [`IArchive`](../../iarchive/) object representing the archive.

### See Also

* interface [IArchive](../../iarchive/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)

---

## GetArchive(Stream) {#getarchive}

Detects the archive format and creates the appropriate [`IArchive`](../../iarchive/) object according to the type of archive specified by the given stream.

```csharp
public static IArchive GetArchive(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream containing the archive data. It must bee seekable. |

### Return Value

An [`IArchive`](../../iarchive/) object representing the archive.

### See Also

* interface [IArchive](../../iarchive/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


