---
title: SevenZipArchiveEntry.Extract
second_title: Aspose.ZIP untuk Referensi .NET API
description: SevenZipArchiveEntry metode. Mengekstrak entri ke sistem file dengan jalur yang disediakan.
type: docs
weight: 80
url: /id/net/aspose.zip.sevenzip/sevenziparchiveentry/extract/
---
## Extract(string, string) {#extract}

Mengekstrak entri ke sistem file dengan jalur yang disediakan.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Jalur ke file tujuan. Jika file sudah ada, itu akan ditimpa. |
| password | String | Kata sandi opsional untuk dekripsi. |

### Nilai Pengembalian

Info file dari file yang dibuat.

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
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Lihat juga

* class [SevenZipArchiveEntry](../)
* ruang nama [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* perakitan [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Mengekstrak entri ke aliran yang disediakan.

```csharp
public void Extract(Stream destination, string password = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| destination | Stream | Aliran tujuan. Harus dapat ditulis. |
| password | String | Kata sandi opsional untuk dekripsi. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | *destination* tidak mendukung penulisan. |
| InvalidOperationException | Arsip tidak dibuka untuk ekstraksi. - atau - Entri ini adalah direktori. |
| InvalidDataException | Data yang salah dalam entri. |

### Contoh

Ekstrak entri arsip zip dengan kata sandi.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Lihat juga

* class [SevenZipArchiveEntry](../)
* ruang nama [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* perakitan [Aspose.Zip](../../../)


