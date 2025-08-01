---
title: Bzip2Archive.Save
second_title: Aspose.ZIP for .NET API Reference
description: Bzip2Archive method. Saves archive to the stream provided
type: docs
weight: 60
url: /net/aspose.zip.bzip2/bzip2archive/save/
---
## Save(Stream, Bzip2SaveOptions) {#save}

Saves archive to the stream provided.

```csharp
public void Save(Stream outputStream, Bzip2SaveOptions saveOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | Stream | Destination stream. |
| saveOptions | Bzip2SaveOptions | Options for saving a bzip2 archive. If not specified, 900 Kb block size would be used. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | The source of data to be archived has not been provided. |
| ArgumentException | *outputStream* is not writable. |
| UnauthorizedAccessException | File source is read-only or is a directory. |
| DirectoryNotFoundException | The specified file source path is invalid, such as being on an unmapped drive. |
| IOException | The File source is already open. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Remarks

*outputStream* must be writable.

## Examples

Write compressed data to http response stream.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### See Also

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, Bzip2SaveOptions) {#save_1}

Saves archive to a destination file provided.

```csharp
public void Save(string destinationFileName, Bzip2SaveOptions saveOptions = null)
```

| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| saveOptions | Bzip2SaveOptions | Options for saving a bzip2 archive. If not specified, 900 Kb block size would be used. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationFileName* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *destinationFileName* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *destinationFileName* is denied. |
| PathTooLongException | The specified *destinationFileName*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *destinationFileName* contains a colon (:) in the middle of the string. |
| ObjectDisposedException | Archive has been disposed and cannot be used. |

## Examples

Writes compressed data to file.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bz2");
}
```

### See Also

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


