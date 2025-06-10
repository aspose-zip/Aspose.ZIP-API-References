---
title: UueArchive.Save
second_title: Aspose.ZIP for .NET API Reference
description: UueArchive method. Saves archive to the stream provided
type: docs
weight: 70
url: /net/aspose.zip.uue/uuearchive/save/
---
## Save(Stream, UueSaveOptions) {#save}

Saves archive to the stream provided.

```csharp
public void Save(Stream outputStream, UueSaveOptions saveOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | Stream | Destination stream. |
| saveOptions | UueSaveOptions | Options for the archive saving. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | Archive has been disposed and cannot be used. |
| InvalidOperationException | The source of data to be archived has not been provided. |
| ArgumentException | *outputStream* is not writable. |
| UnauthorizedAccessException | File source is read-only or is a directory. |
| DirectoryNotFoundException | The specified file source path is invalid, such as being on an unmapped drive. |
| IOException | The File source is already open. |

## Remarks

*outputStream* must be writable.

## Examples

Write compressed data to http response stream.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### See Also

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, UueSaveOptions) {#save_1}

Saves archive to a destination file provided.

```csharp
public void Save(string destinationFileName, UueSaveOptions saveOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| saveOptions | UueSaveOptions | Options for the archive saving. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | Archive has been disposed and cannot be used. |
| ArgumentNullException | *destinationFileName* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *destinationFileName* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *destinationFileName* is denied. |
| PathTooLongException | The specified *destinationFileName*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *destinationFileName* contains a colon (:) in the middle of the string. |

## Examples

Write encoded data to file.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.uue");
}
```

### See Also

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


