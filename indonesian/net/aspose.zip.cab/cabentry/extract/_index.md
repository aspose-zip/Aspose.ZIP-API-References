---
title: CabEntry.Extract
second_title: Aspose.ZIP untuk Referensi .NET API
description: CabEntry metode. Mengekstrak entri ke sistem file dengan jalur yang disediakan.
type: docs
weight: 30
url: /id/net/aspose.zip.cab/cabentry/extract/
---
## Extract(string) {#extract}

Mengekstrak entri ke sistem file dengan jalur yang disediakan.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Jalur ke file tujuan. Jika file sudah ada, itu akan ditimpa. |

### Nilai Pengembalian

Info file dari file yang dibuat.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *path* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Itu*path* kosong, hanya berisi spasi putih, atau berisi karakter yang tidak valid. |
| UnauthorizedAccessException | Akses ke file*path* ditolak. |
| PathTooLongException | Yang ditentukan*path*, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di*path* berisi titik dua (:) di tengah string. |

### Contoh

```csharp
using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### Lihat juga

* class [CabEntry](../)
* ruang nama [Aspose.Zip.Cab](../../cabentry/)
* perakitan [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Mengekstrak entri ke aliran yang disediakan.

```csharp
public void Extract(Stream destination)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| destination | Stream | Aliran tujuan. Harus dapat ditulis. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | *destination* tidak mendukung penulisan. |

### Contoh

Ekstrak entri arsip taksi.

```csharp
using (var archive = new CabArchive("archive.cab"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### Lihat juga

* class [CabEntry](../)
* ruang nama [Aspose.Zip.Cab](../../cabentry/)
* perakitan [Aspose.Zip](../../../)


