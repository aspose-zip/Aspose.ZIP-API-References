---
title: "IArchiveFileEntry.Extract"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode IArchiveFileEntry. Mengekstrak entri ke sistem berkas menggunakan jalur yang diberikan."
type: docs
weight: 30
url: /id/net/aspose.zip/iarchivefileentry/extract/
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

### Lihat Juga

* interface [IArchiveFileEntry](../)
* namespace [Aspose.Zip](../../iarchivefileentry/)
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

### Lihat Juga

* interface [IArchiveFileEntry](../)
* namespace [Aspose.Zip](../../iarchivefileentry/)
* assembly [Aspose.Zip](../../../)


