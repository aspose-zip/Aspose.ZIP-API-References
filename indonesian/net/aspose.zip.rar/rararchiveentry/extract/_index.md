---
title: RarArchiveEntry.Extract
second_title: Aspose.ZIP untuk Referensi .NET API
description: RarArchiveEntry metode. Mengekstrak entri ke sistem file dengan jalur yang disediakan.
type: docs
weight: 90
url: /id/net/aspose.zip.rar/rararchiveentry/extract/
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
| InvalidDataException | Verifikasi CRC atau MAC gagal untuk masuk. |

### Contoh

Ekstrak dua entri arsip rar.

```csharp
using (FileStream rarFile = File.Open("archive.rar", FileMode.Open))
{
    using (RarArchive archive = new RarArchive(rarFile))
    {
        archive.Entries[0].Extract("first.bin", "pass");
        archive.Entries[1].Extract("second.bin", "pass");
    }
}
```

### Lihat juga

* class [RarArchiveEntry](../)
* ruang nama [Aspose.Zip.Rar](../../rararchiveentry/)
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
| InvalidDataException | Verifikasi CRC atau MAC gagal untuk masuk. |
| ArgumentException | *destination* tidak mendukung penulisan. |

### Contoh

Ekstrak entri arsip rar dengan kata sandi.

```csharp
using (FileStream rarFile = File.Open("archive.zip", FileMode.Open))
{
    using (RarArchive archive = new RarArchive(rarFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### Lihat juga

* class [RarArchiveEntry](../)
* ruang nama [Aspose.Zip.Rar](../../rararchiveentry/)
* perakitan [Aspose.Zip](../../../)


