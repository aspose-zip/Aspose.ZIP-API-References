---
title: Bzip2Archive.SetSource
second_title: Aspose.ZIP untuk Referensi .NET API
description: Bzip2Archive metode. Mengatur konten yang akan dikompresi dalam arsip.
type: docs
weight: 60
url: /id/net/aspose.zip.bzip2/bzip2archive/setsource/
---
## SetSource(Stream) {#setsource_3}

Mengatur konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(Stream source)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| source | Stream | Aliran input untuk arsip. |

### Contoh

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00,0xFF }));
    archive.Save("archive.bz2");
}
```

### Lihat juga

* class [Bzip2Archive](../)
* ruang nama [Aspose.Zip.Bzip2](../../bzip2archive/)
* perakitan [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_2}

Mengatur konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| fileInfo | FileInfo | Referensi ke file yang akan dikompresi. |

### Contoh

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.bz2");
}
```

### Lihat juga

* class [Bzip2Archive](../)
* ruang nama [Aspose.Zip.Bzip2](../../bzip2archive/)
* perakitan [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_4}

Mengatur konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(string path)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Path ke file yang akan dikompresi. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *path* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Itu*path* kosong, hanya berisi spasi putih, atau berisi karakter yang tidak valid. |
| UnauthorizedAccessException | Akses ke file*path* ditolak. |
| PathTooLongException | Yang ditentukan*path*, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di*path* berisi titik dua (:) di tengah string. |

### Contoh

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Lihat juga

* class [Bzip2Archive](../)
* ruang nama [Aspose.Zip.Bzip2](../../bzip2archive/)
* perakitan [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource_1}

Mengatur konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| tarArchive | TarArchive | Arsip tar untuk dikompresi. |
| format | TarFormat | Mendefinisikan format tajuk tar. |

### Perkataan

Gunakan metode ini untuk menyusun arsip tar.bz2 bersama.

### Contoh

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

### Lihat juga

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Bzip2Archive](../)
* ruang nama [Aspose.Zip.Bzip2](../../bzip2archive/)
* perakitan [Aspose.Zip](../../../)

---

## SetSource(CpioArchive, CpioFormat) {#setsource}

Mengatur konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(CpioArchive cpioArchive, CpioFormat format = CpioFormat.OldAscii)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| cpioArchive | CpioArchive | Arsip Cpio untuk dikompresi. |
| format | CpioFormat | Mendefinisikan format tajuk cpio. |

### Perkataan

Gunakan metode ini untuk membuat arsip bersama cpio.bz2.

### Contoh

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

### Lihat juga

* class [CpioArchive](../../../aspose.zip.cpio/cpioarchive/)
* enum [CpioFormat](../../../aspose.zip.cpio/cpioformat/)
* class [Bzip2Archive](../)
* ruang nama [Aspose.Zip.Bzip2](../../bzip2archive/)
* perakitan [Aspose.Zip](../../../)


