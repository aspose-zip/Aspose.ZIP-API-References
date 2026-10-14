---
title: "ComHelper.OpenBzip2"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode ComHelper. Memungkinkan aplikasi COM untuk memuat arsip bzip2 dari aliran"
type: docs
weight: 20
url: /id/net/aspose.zip/comhelper/openbzip2/
---
## OpenBzip2(Stream) {#openbzip2}

Mengizinkan aplikasi COM memuat arsip bzip2 dari aliran.

```csharp
public Bzip2Archive OpenBzip2(Stream stream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Objek aliran .NET yang berisi arsip yang akan dimuat. |

### Nilai Kembalian

Objek [`Bzip2Archive`](../../../aspose.zip.bzip2/bzip2archive/) yang mewakili arsip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| InvalidDataException | Byte tanda tangan salah. |

### Lihat Juga

* class [Bzip2Archive](../../../aspose.zip.bzip2/bzip2archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenBzip2(string) {#openbzip2_1}

Mengizinkan aplikasi COM memuat arsip bzip2 dari file.

```csharp
public Bzip2Archive OpenBzip2(string fileName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | String | Nama file arsip yang akan dimuat. |

### Nilai Kembalian

Objek [`Bzip2Archive`](../../../aspose.zip.bzip2/bzip2archive/) yang mewakili arsip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| ArgumentException | Nama file kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| ArgumentNullException | *fileName* adalah `null`. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| FileNotFoundException | Berkas tidak ditemukan. |
| InvalidDataException | Byte tanda tangan salah. |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. |
| UnauthorizedAccessException | Akses ke *fileName* ditolak. |

### Lihat Juga

* class [Bzip2Archive](../../../aspose.zip.bzip2/bzip2archive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


