---
title: GzipArchive.SetSource
second_title: Aspose.ZIP for .NET API Reference
description: GzipArchive method. Sets the content to be compressed within the archive
type: docs
weight: 80
url: /net/aspose.zip.gzip/gziparchive/setsource/
---
## SetSource(Stream) {#setsource_2}

Sets the content to be compressed within the archive.

```csharp
public void SetSource(Stream source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Stream | The input stream for the archive. |

## Examples

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.gz");
}
```

### See Also

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

Sets the content to be compressed within the archive.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileInfo | FileInfo | The reference to a file to be compressed. |

## Examples

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.gz");
}
```

### See Also

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

Sets the content to be compressed within the archive.

```csharp
public void SetSource(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | Path to file to be compressed. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* contains a colon (:) in the middle of the string. |

## Examples

Open an archive from file by path and extract it to a `MemoryStream`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### See Also

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(TarArchive) {#setsource}

Sets the content to be compressed within the archive.

```csharp
public void SetSource(TarArchive tarArchive)
```

| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | TarArchive | Tar archive to be compressed. |

## Remarks

Use this method to compose joint tar.gz archive.

## Examples

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var gzippedArchive = new GzipArchive())
    {
           gzippedArchive.SetSource(tarArchive);
           gzippedArchive.Save("archive.tar.gz");
    }
}
```

### See Also

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


