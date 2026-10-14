---
title: "GzipArchive.SetSource"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode GzipArchive. Menetapkan konten yang akan dikompres dalam arsip"
type: docs
weight: 90
url: /id/net/aspose.zip.gzip/gziparchive/setsource/
---
## SetSource(Stream) {#setsource_2}

Menetapkan konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(Stream source)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | Stream | Stream input untuk arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.gz");
}
```

### Lihat Juga

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

Menetapkan konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileInfo | FileInfo | Referensi ke file yang akan dikompresi. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.gz");
}
```

### Lihat Juga

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

Menetapkan konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke file yang akan dikompres. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Lihat Juga

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(TarArchive) {#setsource}

Menetapkan konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(TarArchive tarArchive)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tarArchive | TarArchive | Arsip Tar yang akan dikompres. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Catatan

Gunakan metode ini untuk menyusun arsip tar.gz gabungan.

## Contoh

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

### Lihat Juga

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


