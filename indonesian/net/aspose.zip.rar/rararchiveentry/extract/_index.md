---
title: "RarArchiveEntry.Extract"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode RarArchiveEntry. Mengekstrak entri ke sistem file menggunakan jalur yang diberikan"
type: docs
weight: 90
url: /id/net/aspose.zip.rar/rararchiveentry/extract/
---
## Extract(string, string) {#extract}

Mengekstrak entri ke sistem file menggunakan jalur yang disediakan.

```csharp
public FileInfo Extract(string path, string password = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke file tujuan. Jika file sudah ada, akan ditimpa. |
| password | String | Password opsional untuk dekripsi. |

### Nilai Kembalian

Info file dari file yang disusun.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| FileNotFoundException | Berkas tidak ditemukan. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| IOException | Berkas sudah terbuka. |
| InvalidDataException | Data rusak. -atau- verifikasi CRC atau MAC gagal untuk entri. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |

## Contoh

Ekstrak dua entri dari arsip rar.

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

### Lihat Juga

* class [RarArchiveEntry](../)
* namespace [Aspose.Zip.Rar](../../rararchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

Mengekstrak entri ke aliran yang disediakan.

```csharp
public void Extract(Stream destination, string password = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | Stream | Stream tujuan. Harus dapat ditulis. |
| password | String | Password opsional untuk dekripsi. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidDataException | Verifikasi CRC atau MAC gagal untuk entri. |
| ArgumentException | *destination* tidak mendukung penulisan. |
| InvalidDataException | Data rusak. -atau- verifikasi CRC atau MAC gagal untuk entri. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |

## Contoh

Ekstrak sebuah entri arsip rar dengan kata sandi.

```csharp
using (FileStream rarFile = File.Open("archive.zip", FileMode.Open))
{
    using (RarArchive archive = new RarArchive(rarFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### Lihat Juga

* class [RarArchiveEntry](../)
* namespace [Aspose.Zip.Rar](../../rararchiveentry/)
* assembly [Aspose.Zip](../../../)


