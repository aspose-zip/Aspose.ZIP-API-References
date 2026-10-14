---
title: "CabArchive.CreateEntries"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode CabArchive. Menambahkan semua file secara rekursif dari direktori yang ditentukan ke dalam arsip."
type: docs
weight: 30
url: /id/net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Menambahkan semua file ke arsip, secara rekursif, dari direktori yang ditentukan.

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| directory | DirectoryInfo | Direktori yang akan dikompresi. |
| includeRootDirectory | Boolean | Menunjukkan apakah nama direktori root harus disertakan dalam jalur entri. |

### Nilai Kembalian

Instansi [`CabArchive`](../) saat ini.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *directory* bernilai null. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| DirectoryNotFoundException | *directory* tidak dapat ditemukan. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses *directory* atau isinya. |
| UnauthorizedAccessException | Akses ke *directory* atau salah satu file-nya ditolak. |
| IOException | Terjadi kesalahan I/O saat mengakses *directory*. |
| PathTooLongException | Jalur entri yang dihasilkan melebihi panjang maksimum yang ditentukan sistem. |
| InvalidOperationException | Arsip telah dipersiapkan untuk ekstraksi dan tidak dapat menambahkan entri. |

## Contoh

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### Lihat Juga

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Menambahkan semua file secara rekursif ke arsip dari jalur direktori yang ditentukan.

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceDirectory | String | Jalur direktori untuk dikompresi. |
| includeRootDirectory | Boolean | Menunjukkan apakah nama direktori root harus disertakan dalam jalur entri. |

### Nilai Kembalian

Instansi [`CabArchive`](../) saat ini.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentNullException | *sourceDirectory* bernilai null. |
| DirectoryNotFoundException | *sourceDirectory* tidak dapat ditemukan. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses *sourceDirectory*. |
| UnauthorizedAccessException | Akses ke *sourceDirectory* ditolak. |
| PathTooLongException | *sourceDirectory* yang ditentukan melebihi panjang maksimum yang ditentukan sistem. |
| ArgumentException | *sourceDirectory* kosong, hanya berisi spasi putih, atau berisi karakter tidak valid. |
| IOException | Terjadi kesalahan I/O saat mengakses *sourceDirectory*. |
| InvalidOperationException | Arsip telah dipersiapkan untuk ekstraksi dan tidak dapat menambahkan entri. |

## Contoh

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### Lihat Juga

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


