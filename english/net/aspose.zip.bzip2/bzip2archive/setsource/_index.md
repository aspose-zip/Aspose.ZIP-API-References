---
title: Bzip2Archive.SetSource
second_title: Aspose.ZIP for .NET API Reference
description: Bzip2Archive method. Sets the content to be compressed within the archive
type: docs
weight: 70
url: /net/aspose.zip.bzip2/bzip2archive/setsource/
---
## SetSource(Stream) {#setsource_3}

Sets the content to be compressed within the archive.

```csharp
public void SetSource(Stream source)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Stream | The input stream for the archive. |

## Examples

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00,0xFF }));
    archive.Save("archive.bz2");
}
```

### See Also

* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_2}

Sets the content to be compressed within the archive.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileInfo | FileInfo | The reference to a file to be compressed. |

## Examples

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.bz2");
}
```

### See Also

* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_4}

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

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### See Also

* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource_1}

Sets the content to be compressed within the archive.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | TarArchive | Tar archive to be compressed. |
| format | TarFormat | Defines tar header format. |

## Remarks

Use this method to compose joint tar.bz2 archive.

## Examples

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(tarArchive);
        bzippedArchive.Save("archive.tar.bz2");
    }
}
```

### See Also

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(CpioArchive, CpioFormat) {#setsource}

Sets the content to be compressed within the archive.

```csharp
public void SetSource(CpioArchive cpioArchive, CpioFormat format = CpioFormat.OldAscii)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cpioArchive | CpioArchive | Cpio archive to be compressed. |
| format | CpioFormat | Defines cpio header format. |

## Remarks

Use this method to compose joint cpio.bz2 archive.

## Examples

```csharp
using (var cpioArchive = new CpioArchive())
{
    cpioArchive.CreateEntry("first.bin", "data1.bin");
    cpioArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(cpioArchive);
        bzippedArchive.Save("archive.cpio.bz2");
    }
}
```

### See Also

* class [CpioArchive](../../../aspose.zip.cpio/cpioarchive/)
* enum [CpioFormat](../../../aspose.zip.cpio/cpioformat/)
* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


