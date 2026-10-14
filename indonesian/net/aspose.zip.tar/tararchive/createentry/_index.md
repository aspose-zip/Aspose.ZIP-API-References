---
title: "TarArchive.CreateEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode TarArchive. Membuat satu entri dalam arsip"
type: docs
weight: 110
url: /id/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

Buat satu entri dalam arsip.

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| source | Stream | Aliran masukan untuk entri. |
| fileInfo | FileSystemInfo | Metadata file atau folder yang akan dikompresi. |

### Nilai Kembalian

Instansi entri Tar.

### Pengecualian

| exception | kondisi |
| --- | --- |
| PathTooLongException | *name* terlalu panjang untuk tar menurut standar IEEE 1003.1-1998. |
| ArgumentException | Nama file, sebagai bagian dari *name*, melebihi 100 simbol. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan |

## Catatan

Nama entri hanya diatur melalui parameter *name*. Nama file yang diberikan pada parameter *fileInfo* tidak memengaruhi nama entri.

*fileInfo* can refer to DirectoryInfo if the entry is directory.

## Contoh

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### Lihat Juga

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Buat satu entri dalam arsip.

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| fileInfo | FileInfo | Metadata file atau folder yang akan dikompresi. |
| openImmediately | Boolean | True, jika membuka file segera, jika tidak membuka file saat menyimpan arsip. |

### Nilai Kembalian

Instansi entri Tar.

### Pengecualian

| exception | kondisi |
| --- | --- |
| PathTooLongException | *name* terlalu panjang untuk tar menurut standar IEEE 1003.1-1998. |
| ArgumentException | Nama file, sebagai bagian dari *name*, melebihi 100 simbol. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan |

## Catatan

Nama entri hanya diatur melalui parameter *name*. Nama file yang diberikan pada parameter *fileInfo* tidak memengaruhi nama entri.

*fileInfo* can refer to DirectoryInfo if the entry is directory.

Jika file dibuka segera dengan parameter *openImmediately*, file akan diblokir sampai arsip dibuang.

## Contoh

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### Lihat Juga

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Buat satu entri dalam arsip.

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| path | String | Jalur ke file yang akan dikompres. |
| openImmediately | Boolean | True, jika membuka file segera, jika tidak membuka file saat menyimpan arsip. |

### Nilai Kembalian

Instansi entri Tar.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. - atau - Nama file, sebagai bagian dari *name*, melebihi 100 simbol. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. - atau - *name* terlalu panjang untuk tar menurut standar IEEE 1003.1-1998. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan |

## Catatan

Nama entri hanya diatur melalui parameter *name*. Nama file yang diberikan dalam parameter *path* tidak memengaruhi nama entri.

Jika file dibuka segera dengan parameter *openImmediately*, file akan diblokir sampai arsip dibuang.

## Contoh

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### Lihat Juga

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


