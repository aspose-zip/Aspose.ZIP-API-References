---
title: "ArchiveEntry.Extract"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode ArchiveEntry. Mengekstrak entri ke sistem file menggunakan jalur yang diberikan"
type: docs
weight: 110
url: /id/net/aspose.zip/archiveentry/extract/
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
| ObjectDisposedException | Dilempar jika arsip telah dibuang. |

## Contoh

Ekstrak dua entri dari arsip ZIP, masing-masing dengan kata sandi sendiri

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract("first.bin", "first_pass");
        archive.Entries[1].Extract("second.bin", "second_pass");
    }
}
```

### Lihat Juga

* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
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
| InvalidDataException | Data rusak. -atau- verifikasi CRC atau MAC gagal untuk entri. |
| IOException | Sumber rusak atau tidak dapat dibaca. |
| ArgumentException | *destination* tidak mendukung penulisan. |
| ObjectDisposedException | Dilempar jika arsip telah dibuang. |

## Contoh

Ekstrak sebuah entri dari arsip zip dengan kata sandi.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Open))
{
    using (Archive archive = new Archive(zipFile))
    {
        archive.Entries[0].Extract(httpResponseStream, "p@s$");
    }
}
```

### Lihat Juga

* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


