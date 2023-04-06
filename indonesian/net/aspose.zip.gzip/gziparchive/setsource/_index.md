---
title: GzipArchive.SetSource
second_title: Aspose.ZIP untuk Referensi .NET API
description: GzipArchive metode. Mengatur konten yang akan dikompresi dalam arsip.
type: docs
weight: 70
url: /id/net/aspose.zip.gzip/gziparchive/setsource/
---
## SetSource(Stream) {#setsource_2}

Mengatur konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(Stream source)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| source | Stream | Aliran input untuk arsip. |

### Contoh

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.gz");
}
```

### Lihat juga

* class [GzipArchive](../)
* ruang nama [Aspose.Zip.Gzip](../../gziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

Mengatur konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| fileInfo | FileInfo | Referensi ke file yang akan dikompresi. |

### Contoh

Buka arsip dari aliran dan ekstrak ke a`MemoryStream`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.gz");
}
```

### Lihat juga

* class [GzipArchive](../)
* ruang nama [Aspose.Zip.Gzip](../../gziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

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

Buka arsip dari file dengan jalur dan ekstrak ke a`MemoryStream`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Lihat juga

* class [GzipArchive](../)
* ruang nama [Aspose.Zip.Gzip](../../gziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## SetSource(TarArchive) {#setsource}

Mengatur konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(TarArchive tarArchive)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| tarArchive | TarArchive | Arsip tar untuk dikompresi. |

### Perkataan

Gunakan metode ini untuk menyusun arsip tar.gz bersama.

### Contoh

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

### Lihat juga

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* class [GzipArchive](../)
* ruang nama [Aspose.Zip.Gzip](../../gziparchive/)
* perakitan [Aspose.Zip](../../../)


