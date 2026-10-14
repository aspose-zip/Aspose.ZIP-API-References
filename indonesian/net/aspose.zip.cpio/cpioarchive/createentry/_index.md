---
title: "CpioArchive.CreateEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode CpioArchive. Membuat satu entri tunggal di dalam arsip"
type: docs
weight: 40
url: /id/net/aspose.zip.cpio/cpioarchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

Buat satu entri dalam arsip.

```csharp
public CpioEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| fileInfo | FileInfo | Metadata file atau folder yang akan dikompresi. |
| openImmediately | Boolean | True, jika membuka file segera, jika tidak membuka file saat menyimpan arsip. |

### Nilai Kembalian

Instansi entri Cpio.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *name* bernilai null. |
| ArgumentException | *name* kosong. |
| ArgumentNullException | *fileInfo* bernilai null. |
| ObjectDisposedException | Dilemparkan ketika arsip telah dibuang. |

## Catatan

Jika file dibuka segera dengan parameter *openImmediately*, file akan diblokir sampai arsip dibuang.

## Contoh

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new CpioArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.cpio");
}
```

### Lihat Juga

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

Buat satu entri dalam arsip.

```csharp
public CpioEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| sourcePath | String | Jalur ke file yang akan dikompres. |
| openImmediately | Boolean | True, jika membuka file segera, jika tidak membuka file saat menyimpan arsip. |

### Nilai Kembalian

Instansi entri Cpio.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *sourcePath* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *sourcePath* kosong, hanya berisi spasi, atau mengandung karakter tidak valid. - atau - Nama file, sebagai bagian dari *name*, melebihi 100 simbol. |
| UnauthorizedAccessException | Akses ke file *sourcePath* ditolak. |
| PathTooLongException | *sourcePath* yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. - atau - *name* terlalu panjang untuk cpio. |
| NotSupportedException | File di *sourcePath* mengandung tanda titik dua (:) di tengah string. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Catatan

Nama entri hanya ditetapkan melalui parameter *name*. Nama file yang diberikan dalam parameter *sourcePath* tidak memengaruhi nama entri.

Jika file dibuka segera dengan parameter *openImmediately*, file akan diblokir sampai arsip dibuang.

## Contoh

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### Lihat Juga

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Buat satu entri dalam arsip.

```csharp
public CpioEntry CreateEntry(string name, Stream source)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| source | Stream | Aliran masukan untuk entri. |

### Nilai Kembalian

Instansi entri Cpio.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *name* bernilai null. |
| ArgumentNullException | *source* bernilai null. |
| ArgumentException | *name* kosong. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.cpio");
}
```

### Lihat Juga

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


