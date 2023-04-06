---
title: SharArchive.CreateEntry
second_title: Aspose.ZIP untuk Referensi .NET API
description: SharArchive metode. Buat satu entri dalam arsip.
type: docs
weight: 40
url: /id/net/aspose.zip.shar/shararchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

Buat satu entri dalam arsip.

```csharp
public SharEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| name | String | Nama entri. |
| fileInfo | FileInfo | Metadata file atau folder yang akan dikompresi. |
| openImmediately | Boolean | Benar jika langsung buka file, jika tidak buka file di penyimpanan arsip. |

### Nilai Pengembalian

Contoh entri Shar.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *name* adalah nol. |
| ArgumentException | *name* kosong. |
| ArgumentNullException | *fileInfo* adalah nol. |

### Perkataan

Jika file segera dibuka dengan*openImmediately*parameter itu menjadi diblokir sampai arsip dibuang.

### Contoh

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new SharArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.shar");
}
```

### Lihat juga

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* ruang nama [Aspose.Zip.Shar](../../shararchive/)
* perakitan [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Buat satu entri dalam arsip.

```csharp
public SharEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| name | String | Nama entri. |
| sourcePath | String | Path ke file yang akan dikompresi. |
| openImmediately | Boolean | Benar jika langsung buka file, jika tidak buka file di penyimpanan arsip. |

### Nilai Pengembalian

Contoh entri Shar.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *sourcePath* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Itu*sourcePath* kosong, hanya berisi spasi putih, atau berisi karakter yang tidak valid. - atau - Nama file, sebagai bagian dari*name*, melebihi 100 simbol. |
| UnauthorizedAccessException | Akses ke file*sourcePath* ditolak. |
| PathTooLongException | Yang ditentukan*sourcePath* , nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. - atau -*name* terlalu panjang untuk shar. |
| NotSupportedException | Berkas di*sourcePath* berisi titik dua (:) di tengah string. |

### Perkataan

Nama entri hanya diatur di dalam*name* parameter. Nama file yang disediakan di*sourcePath* parameter tidak mempengaruhi nama entri.

Jika file segera dibuka dengan*openImmediately*parameter itu menjadi diblokir sampai arsip dibuang.

### Contoh

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Lihat juga

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* ruang nama [Aspose.Zip.Shar](../../shararchive/)
* perakitan [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Buat satu entri dalam arsip.

```csharp
public SharEntry CreateEntry(string name, Stream source)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| name | String | Nama entri. |
| source | Stream | Aliran input untuk entri. |

### Nilai Pengembalian

Contoh entri Shar.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *name* adalah nol. |
| ArgumentNullException | *source* adalah nol. |
| ArgumentException | *name* kosong. |

### Contoh

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.shar");
}
```

### Lihat juga

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* ruang nama [Aspose.Zip.Shar](../../shararchive/)
* perakitan [Aspose.Zip](../../../)


