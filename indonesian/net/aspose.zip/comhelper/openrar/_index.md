---
title: "ComHelper.OpenRar"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode ComHelper. Memungkinkan aplikasi COM untuk memuat arsip rar dari aliran"
type: docs
weight: 40
url: /id/net/aspose.zip/comhelper/openrar/
---
## OpenRar(Stream) {#openrar}

Mengizinkan aplikasi COM untuk memuat arsip rar dari sebuah aliran.

```csharp
public RarArchive OpenRar(Stream stream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Objek aliran .NET yang berisi arsip yang akan dimuat. |

### Nilai Kembalian

Objek [`RarArchive`](../../../aspose.zip.rar/rararchive/) yang mewakili arsip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidDataException | Dilemparkan ketika data tidak valid atau rusak. |

### Lihat Juga

* class [RarArchive](../../../aspose.zip.rar/rararchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)

---

## OpenRar(string) {#openrar_1}

Mengizinkan aplikasi COM untuk memuat arsip rar dari sebuah file.

```csharp
public RarArchive OpenRar(string fileName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | String | Nama file arsip yang akan dimuat. |

### Nilai Kembalian

Objek [`RarArchive`](../../../aspose.zip.rar/rararchive/) yang mewakili arsip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | Nama file kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| ArgumentNullException | *fileName* adalah `null`. |
| Exception | Dilemparkan ketika terjadi kesalahan runtime. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| FileNotFoundException | Berkas tidak ditemukan. |
| InvalidDataException | Dilemparkan ketika data tidak valid atau rusak. |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. |
| UnauthorizedAccessException | Akses ke *fileName* ditolak. |

### Lihat Juga

* class [RarArchive](../../../aspose.zip.rar/rararchive/)
* class [ComHelper](../)
* namespace [Aspose.Zip](../../comhelper/)
* assembly [Aspose.Zip](../../../)


