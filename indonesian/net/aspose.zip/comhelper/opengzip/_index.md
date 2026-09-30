---
title: "ComHelper.OpenGzip"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode ComHelper. Memungkinkan aplikasi COM untuk memuat arsip gzip dari aliran"
type: docs
weight: 30
url: /id/net/aspose.zip/comhelper/opengzip/
---
## OpenGzip(Stream) {#opengzip}

Mengizinkan aplikasi COM memuat arsip gzip dari aliran.

```csharp
public GzipArchive OpenGzip(Stream stream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Objek aliran .NET yang berisi arsip yang akan dimuat. |

### Nilai Kembalian

Objek [`GzipArchive`](../../../aspose.zip.gzip/gziparchive/) yang mewakili arsip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ArgumentNullException | Dilempar ketika *stream* bernilai null. |
| InvalidDataException | Dilemparkan ketika data tidak valid atau rusak. |

### Lihat Juga

* class [GzipArchive](../../../aspose.zip.gzip/gziparchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenGzip(string) {#opengzip_1}

Mengizinkan aplikasi COM untuk memuat arsip gzip dari sebuah file.

```csharp
public GzipArchive OpenGzip(string fileName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | String | Nama file arsip yang akan dimuat. |

### Nilai Kembalian

Objek [`GzipArchive`](../../../aspose.zip.gzip/gziparchive/) yang mewakili arsip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ArgumentException | Nama file kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| ArgumentNullException | *fileName* adalah `null`. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| FileNotFoundException | Berkas tidak ditemukan. |
| InvalidDataException | Dilemparkan ketika data tidak valid atau rusak. |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. |
| UnauthorizedAccessException | Akses ke *fileName* ditolak. |

### Lihat Juga

* class [GzipArchive](../../../aspose.zip.gzip/gziparchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


