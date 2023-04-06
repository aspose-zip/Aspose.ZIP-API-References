---
title: XarFileEntry.Extract
second_title: Aspose.ZIP untuk Referensi .NET API
description: XarFileEntry metode. Mengekstrak entri ke sistem file dengan jalur yang disediakan.
type: docs
weight: 20
url: /id/net/aspose.zip.xar/xarfileentry/extract/
---
## Extract(string) {#extract}

Mengekstrak entri ke sistem file dengan jalur yang disediakan.

```csharp
public abstract FileInfo Extract(string path)
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
using (var archive = new XarArchive("archive.xar"))
{
    archive.Entries.First().Extract("data.bin");
}
```

### Lihat juga

* class [XarFileEntry](../)
* ruang nama [Aspose.Zip.Xar](../../xarfileentry/)
* perakitan [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Mengekstrak entri ke aliran yang disediakan.

```csharp
public abstract void Extract(Stream destination)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| destination | Stream | Aliran tujuan. Harus dapat ditulis. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | *destination* tidak mendukung penulisan. |

### Contoh

Ekstrak entri arsip wim.

```csharp
using (var archive = new WimArchive("archive.wim"))
{
    archive.Images[0].RootDirectory.Files[0].Extract(httpResponseStream);
}
```

### Lihat juga

* class [XarFileEntry](../)
* ruang nama [Aspose.Zip.Xar](../../xarfileentry/)
* perakitan [Aspose.Zip](../../../)


