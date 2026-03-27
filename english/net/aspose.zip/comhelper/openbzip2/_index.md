---
title: ComHelper.OpenBzip2
second_title: Aspose.ZIP for .NET API Reference
description: ComHelper method. Allows a COM application to load a bzip2 archive from a stream
type: docs
weight: 20
url: /net/aspose.zip/comhelper/openbzip2/
---
## OpenBzip2(Stream) {#openbzip2}

Allows a COM application to load a bzip2 archive from a stream.

```csharp
public Bzip2Archive OpenBzip2(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | A .NET stream object that contains the archive to load. |

### Return Value

A [`Bzip2Archive`](../../../aspose.zip.bzip2/bzip2archive/) object that represents the archive.

### Exceptions

| exception | condition |
| --- | --- |
| EndOfStreamException | Thrown when the end of the stream is reached before the expected number of bytes are read. |
| InvalidDataException | Wrong signature bytes. |

### See Also

* class [Bzip2Archive](../../../aspose.zip.bzip2/bzip2archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenBzip2(string) {#openbzip2_1}

Allows a COM application to load a bzip2 archive from a file.

```csharp
public Bzip2Archive OpenBzip2(string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | Filename of the archive to load. |

### Return Value

A [`Bzip2Archive`](../../../aspose.zip.bzip2/bzip2archive/) object that represents the archive.

### Exceptions

| exception | condition |
| --- | --- |
| EndOfStreamException | Thrown when the end of the stream is reached before the expected number of bytes are read. |
| ArgumentException | The file name is empty, contains only white spaces, or contains invalid characters. |
| ArgumentNullException | *fileName* is `null`. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| FileNotFoundException | The file is not found. |
| InvalidDataException | Wrong signature bytes. |
| PathTooLongException | The specified path, file name, or both exceed the system-defined maximum length. |
| UnauthorizedAccessException | Access to *fileName* is denied. |

### See Also

* class [Bzip2Archive](../../../aspose.zip.bzip2/bzip2archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


