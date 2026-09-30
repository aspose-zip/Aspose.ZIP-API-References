---
title: "ComHelper.OpenZip"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode ComHelper. Memungkinkan aplikasi COM memuat arsip ZIP dari sebuah *stream*"
type: docs
weight: 50
url: /id/net/aspose.zip/comhelper/openzip/
---
## OpenZip(Stream) {#openzip}

Mengizinkan aplikasi COM untuk memuat arsip ZIP dari sebuah aliran.

```csharp
public Archive OpenZip(Stream stream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Objek aliran .NET yang berisi arsip yang akan dimuat. |

### Nilai Kembalian

Sebuah objek [`Archive`](../../archive/) yang mewakili arsip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |

### Lihat Juga

* class [Archive](../../archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenZip(string) {#openzip_1}

Mengizinkan aplikasi COM untuk memuat arsip ZIP dari sebuah file.

```csharp
public Archive OpenZip(string fileName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | String | Nama file arsip yang akan dimuat. |

### Nilai Kembalian

Sebuah objek [`Archive`](../../archive/) yang mewakili arsip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ArgumentException | Nama file kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| ArgumentNullException | *fileName* adalah `null`. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| FileNotFoundException | Berkas tidak ditemukan. |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. |
| UnauthorizedAccessException | Akses ke *fileName* ditolak. |

### Lihat Juga

* class [Archive](../../archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


