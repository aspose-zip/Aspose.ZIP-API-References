---
title: UueArchive.SetSource
second_title: Aspose.ZIP for .NET API Reference
description: UueArchive method. Sets the content to be encoded within the archive
type: docs
weight: 80
url: /net/aspose.zip.uue/uuearchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Sets the content to be encoded within the archive.

```csharp
public void SetSource(Stream source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Stream | The input stream for the archive. |

## Examples

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.uue");
}
```

### See Also

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

Sets the content to be compressed within the archive.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileInfo | FileInfo | The reference to a file to be compressed. |

## Examples

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.uue");
}
```

### See Also

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Sets the content to be encoded within the archive.

```csharp
public void SetSource(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | Path to file to be encoded. |

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

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### See Also

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


