---
title: "IsoEntry.Extract"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode IsoEntry. Mengekstrak entri ke sistem file menggunakan jalur yang diberikan"
type: docs
weight: 50
url: /id/net/aspose.zip.iso/isoentry/extract/
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

Instansi FileInfo yang berisi data yang diekstrak.

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
| InvalidOperationException | Header arsip dan informasi layanan tidak dibaca. |

### Lihat Juga

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
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
| NotSupportedException | Muncul jika entri tidak mewakili sebuah file. |
| ArgumentException | Stream yang diberikan tidak mendukung penulisan. |

### Lihat Juga

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)


