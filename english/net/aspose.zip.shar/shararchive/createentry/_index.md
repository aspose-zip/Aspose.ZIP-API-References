---
title: CreateEntry
second_title: Aspose.ZIP for .NET API Reference
description: 
type: docs
weight: 30
url: /net/aspose.zip.shar/shararchive/createentry/
---
## SharArchive.CreateEntry method (1 of 3)

Create single entry within the archive.

```csharp
public SharEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| fileInfo | FileInfo | The metadata of file or folder to be compressed. |
| openImmediately | Boolean | True if open the file immediately, otherwise open the file on archive saving. |

### Return Value

Shar entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *name* is null. |
| ArgumentException | *name* is empty. |
| ArgumentNullException | *fileInfo* is null. |

### Remarks

If the file is opened immediately with *openImmediately* parameter it becomes blocked until archive is disposed.

### Examples

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new SharArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.shar");
}
```

### See Also

* class [SharEntry](../../sharentry)
* class [SharArchive](../../shararchive)
* namespace [Aspose.Zip.Shar](../../shararchive)
* assembly [Aspose.Zip](../../../)

---

## SharArchive.CreateEntry method (2 of 3)

Create single entry within the archive.

```csharp
public SharEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| sourcePath | String | Path to file to be compressed. |
| openImmediately | Boolean | True if open the file immediately, otherwise open the file on archive saving. |

### Return Value

Shar entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourcePath* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *sourcePath* is empty, contains only white spaces, or contains invalid characters. - or - File name, as a part of *name*, exceeds 100 symbols. |
| UnauthorizedAccessException | Access to file *sourcePath* is denied. |
| PathTooLongException | The specified *sourcePath*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. - or - *name* is too long for shar. |
| NotSupportedException | File at *sourcePath* contains a colon (:) in the middle of the string. |

### Remarks

The entry name is solely set within *name* parameter. The file name provided in *sourcePath* parameter does not affect the entry name.

If the file is opened immediately with *openImmediately* parameter it becomes blocked until archive is disposed.

### Examples

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### See Also

* class [SharEntry](../../sharentry)
* class [SharArchive](../../shararchive)
* namespace [Aspose.Zip.Shar](../../shararchive)
* assembly [Aspose.Zip](../../../)

---

## SharArchive.CreateEntry method (3 of 3)

Create single entry within the archive.

```csharp
public SharEntry CreateEntry(string name, Stream source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the entry. |
| source | Stream | The input stream for the entry. |

### Return Value

Shar entry instance.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *name* is null. |
| ArgumentNullException | *source* is null. |
| ArgumentException | *name* is empty. |

### Examples

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.shar");
}
```

### See Also

* class [SharEntry](../../sharentry)
* class [SharArchive](../../shararchive)
* namespace [Aspose.Zip.Shar](../../shararchive)
* assembly [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.ZIP.dll -->