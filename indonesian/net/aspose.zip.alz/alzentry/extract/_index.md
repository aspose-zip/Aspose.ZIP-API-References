---
title: "AlzEntry.Extract"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "AlzEntry method. Mengekstrak entri ke sistem file menggunakan jalur yang diberikan"
type: docs
weight: 60
url: /id/net/aspose.zip.alz/alzentry/extract/
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
| InvalidDataException | Arsip rusak. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| ObjectDisposedException | Dilemparkan jika aliran sumber telah dibuang. |
| FileNotFoundException | Berkas tidak ditemukan. |

## Contoh

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Lihat Juga

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
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
| ArgumentException | *destination* tidak mendukung penulisan. |
| InvalidOperationException | Arsip tidak dibuka untuk ekstraksi. - atau - Entri ini adalah direktori. |
| InvalidDataException | Data salah dalam entri. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |

## Contoh

Ekstrak entri arsip ALZ dengan kata sandi.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Lihat Juga

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)


