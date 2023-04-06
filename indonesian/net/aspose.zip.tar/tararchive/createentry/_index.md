---
title: TarArchive.CreateEntry
second_title: Aspose.ZIP untuk Referensi .NET API
description: TarArchive metode. Buat satu entri dalam arsip.
type: docs
weight: 80
url: /id/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

Buat satu entri dalam arsip.

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| name | String | Nama entri. |
| source | Stream | Aliran input untuk entri. |
| fileInfo | FileSystemInfo | Metadata file atau folder yang akan dikompresi. |

### Nilai Pengembalian

Contoh entri tar.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| PathTooLongException | *name* terlalu panjang untuk tar pada standar IEEE 1003.1-1998. |
| ArgumentException | Nama file, sebagai bagian dari*name*, melebihi 100 simbol. |

### Perkataan

Nama entri hanya diatur di dalam*name* parameter. Nama file yang disediakan di*fileInfo* parameter tidak mempengaruhi nama entri.

*fileInfo* dapat merujuk keDirectoryInfo jika entri adalah direktori.

### Contoh

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### Lihat juga

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* ruang nama [Aspose.Zip.Tar](../../tararchive/)
* perakitan [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Buat satu entri dalam arsip.

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| name | String | Nama entri. |
| fileInfo | FileInfo | Metadata file atau folder yang akan dikompresi. |
| openImmediately | Boolean | Benar jika langsung buka file, jika tidak buka file di penyimpanan arsip. |

### Nilai Pengembalian

Contoh entri tar.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| PathTooLongException | *name* terlalu panjang untuk tar pada standar IEEE 1003.1-1998. |
| ArgumentException | Nama file, sebagai bagian dari*name*, melebihi 100 simbol. |

### Perkataan

Nama entri hanya diatur di dalam*name* parameter. Nama file yang disediakan di*fileInfo* parameter tidak mempengaruhi nama entri.

*fileInfo* dapat merujuk keDirectoryInfo jika entri adalah direktori.

Jika file segera dibuka dengan*openImmediately*parameter itu menjadi diblokir sampai arsip dibuang.

### Contoh

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### Lihat juga

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* ruang nama [Aspose.Zip.Tar](../../tararchive/)
* perakitan [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Buat satu entri dalam arsip.

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| name | String | Nama entri. |
| path | String | Path ke file yang akan dikompresi. |
| openImmediately | Boolean | Benar jika langsung buka file, jika tidak buka file di penyimpanan arsip. |

### Nilai Pengembalian

Contoh entri tar.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *path* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Itu*path* kosong, hanya berisi spasi putih, atau berisi karakter yang tidak valid. - atau - Nama file, sebagai bagian dari*name*, melebihi 100 simbol. |
| UnauthorizedAccessException | Akses ke file*path* ditolak. |
| PathTooLongException | Yang ditentukan*path* , nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. - atau -*name* terlalu panjang untuk tar pada standar IEEE 1003.1-1998. |
| NotSupportedException | Berkas di*path* berisi titik dua (:) di tengah string. |

### Perkataan

Nama entri hanya diatur di dalam*name* parameter. Nama file yang disediakan di*path* parameter tidak mempengaruhi nama entri.

Jika file segera dibuka dengan*openImmediately*parameter itu menjadi diblokir sampai arsip dibuang.

### Contoh

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### Lihat juga

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* ruang nama [Aspose.Zip.Tar](../../tararchive/)
* perakitan [Aspose.Zip](../../../)


