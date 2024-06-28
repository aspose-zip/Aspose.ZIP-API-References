---
title: CpioArchive.CpioArchive
second_title: Aspose.ZIP for .NET API Reference
description: CpioArchive constructor. Initializes a new instance of the CpioArchive class
type: docs
weight: 10
url: /net/aspose.zip.cpio/cpioarchive/cpioarchive/
---
## CpioArchive() {#constructor}

Initializes a new instance of the [`CpioArchive`](../) class.

```csharp
public CpioArchive()
```

## Examples

The following example shows how to compress a file.

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### See Also

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## CpioArchive(Stream) {#constructor_1}

Initializes a new instance of the [`CpioArchive`](../) class and composes entries list can be extracted from the archive.

```csharp
public CpioArchive(Stream sourceStream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | The source of the archive. It must be seekable. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceStream* is null. |
| ArgumentException | *sourceStream* is not seekable. |
| InvalidDataException | *sourceStream* is not valid cpio archive. |

## Remarks

This constructor does not unpack any entry. See [`Open`](../../cpioentry/open/) method for unpacking.

## Examples

The following example shows how to extract all of the entries to a directory.

```csharp
using (var archive = new CpioArchive(File.OpenRead("archive.cpio")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### See Also

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## CpioArchive(string) {#constructor_2}

Initializes a new instance of the [`CpioArchive`](../) class and composes entries list can be extracted from the archive.

```csharp
public CpioArchive(string path)
```

| Parameter | Type | Description |
| --- | --- | --- |
| path | String | The path to the archive file. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* is null. |
| SecurityException | The caller does not have the required permission to access. |
| ArgumentException | The *path* is empty, contains only white spaces, or contains invalid characters. |
| UnauthorizedAccessException | Access to file *path* is denied. |
| PathTooLongException | The specified *path*, file name, or both exceed the system-defined maximum length. For example, on Windows-based platforms, paths must be less than 248 characters, and file names must be less than 260 characters. |
| NotSupportedException | File at *path* contains a colon (:) in the middle of the string. |
| FileNotFoundException | The file is not found. |
| DirectoryNotFoundException | The specified path is invalid, such as being on an unmapped drive. |
| IOException | The file is already open. |

## Remarks

This constructor does not unpack any entry. See [`Open`](../../cpioentry/open/) method for unpacking.

## Examples

The following example shows how to extract all of the entries to a directory.

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### See Also

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


