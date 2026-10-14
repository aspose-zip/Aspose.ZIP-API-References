---
title: "GzipArchive.Extract"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode GzipArchive. Mengekstrak arsip ke aliran yang diberikan"
type: docs
weight: 50
url: /id/net/aspose.zip.gzip/gziparchive/extract/
---
## Extract(Stream) {#extract_1}

Mengekstrak arsip ke aliran yang disediakan.

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
| InvalidDataException | Aliran rusak dan tidak berisi data yang valid. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |

## Contoh

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
     archive.Extract(httpResponseStream);
}
```

### Lihat Juga

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Mengekstrak arsip ke file berdasarkan jalur.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke file tujuan. Jika file sudah ada, akan ditimpa. |

### Nilai Kembalian

Info file yang diekstrak.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| InvalidDataException | Aliran rusak dan tidak berisi data yang valid. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

### Lihat Juga

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


