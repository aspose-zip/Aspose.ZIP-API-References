---
title: "LzxArchiveEntry.Extract"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "LzxArchiveEntry metode. Mengekstrak entri arsip Lzx ke sistem file dengan jalur"
type: docs
weight: 80
url: /id/net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

Mengekstrak entri arsip Lzx ke sistem berkas berdasarkan jalur.

```csharp
public FileSystemInfo Extract(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke file yang akan menyimpan data terdekompresi. |

### Nilai Kembalian

FileSystemInfoInstance yang berisi data yang diekstrak.

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidOperationException | Header arsip dan informasi layanan tidak dibaca. |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| InvalidDataException | Checksum tidak cocok untuk header atau data. - atau - Arsip rusak. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| NotSupportedException | Metode kompresi tidak valid. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai secara tak terduga. |

## Contoh

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Lihat Juga

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Mengekstrak entri ke aliran yang disediakan.

```csharp
public void Extract(Stream destination)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | Stream | Stream tujuan. Harus dapat ditulis. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *destination* tidak mendukung penulisan. |
| InvalidDataException | Checksum tidak cocok untuk header atau data. - atau - Arsip rusak. |
| ArgumentNullException | Aliran tujuan bernilai null. |
| NotSupportedException | Metode kompresi tidak valid. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai secara tak terduga. |

### Lihat Juga

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


