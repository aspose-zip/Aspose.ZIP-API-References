---
title: ComHelper.OpenZip
second_title: Aspose.ZIP for .NET API Reference
description: ComHelper method. Allows a COM application to load a ZIP archive from a stream
type: docs
weight: 50
url: /net/aspose.zip/comhelper/openzip/
---
## OpenZip(Stream) {#openzip}

Allows a COM application to load a ZIP archive from a stream.

```csharp
public Archive OpenZip(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | A .NET stream object that contains the archive to load. |

### Return Value

A [`Archive`](../../archive/) object that represents the archive.

### Exceptions

| exception | condition |
| --- | --- |
| EndOfStreamException | Thrown when the end of the stream is reached before the expected number of bytes are read. |

### See Also

* class [Archive](../../archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenZip(string) {#openzip_1}

Allows a COM application to load a ZIP archive from a file.

```csharp
public Archive OpenZip(string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | Filename of the archive to load. |

### Return Value

A [`Archive`](../../archive/) object that represents the archive.

### Exceptions

| exception | condition |
| --- | --- |
| EndOfStreamException | Thrown when the end of the stream is reached before the expected number of bytes are read. |
| ArgumentException | The file name is empty, contains only white spaces, or contains invalid characters. |
| ArgumentNullException | *fileName* is `null`. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| FileNotFoundException | The file is not found. |
| PathTooLongException | The specified path, file name, or both exceed the system-defined maximum length. |
| UnauthorizedAccessException | Access to *fileName* is denied. |

### See Also

* class [Archive](../../archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


