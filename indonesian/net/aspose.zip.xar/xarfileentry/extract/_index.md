---
title: "XarFileEntry.Extract"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "XarFileEntry method. Mengekstrak entri ke sistem berkas menggunakan jalur yang diberikan"
type: docs
weight: 30
url: /id/net/aspose.zip.xar/xarfileentry/extract/
---
## Extract(string) {#extract}

Mengekstrak entri ke sistem file menggunakan jalur yang disediakan.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke file tujuan. Jika file sudah ada, akan ditimpa. |

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
| InvalidDataException | Arsip rusak. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| FileNotFoundException | Berkas tidak ditemukan. |
| IOException | Terjadi kesalahan I/O. -atau- Thread lain mungkin telah menyebabkan perubahan tak terduga pada posisi handle file sistem operasi. |

## Contoh

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    ((XarFileEntry)archive.Entries[0]).Extract("data.bin");
}
```

### Lihat Juga

* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
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
| InvalidDataException | Arsip rusak. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |

## Contoh

Ekstrak sebuah entri dari arsip xar.

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    ((XarFileEntry)archive.Entries[0]).Extract(httpResponseStream);
}
```

### Lihat Juga

* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


