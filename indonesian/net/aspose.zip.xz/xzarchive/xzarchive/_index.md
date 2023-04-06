---
title: XzArchive.XzArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: XzArchive konstruktor. Menginisialisasi instance baru dariXzArchive kelas dan menyusun arsip dalam format xz.
type: docs
weight: 10
url: /id/net/aspose.zip.xz/xzarchive/xzarchive/
---
## XzArchive(XzArchiveSettings) {#constructor}

Menginisialisasi instance baru dari[`XzArchive`](../) kelas dan menyusun arsip dalam format xz.

```csharp
public XzArchive(XzArchiveSettings settings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| settings | XzArchiveSettings | Kumpulan pengaturan arsip xz tertentu: ukuran kamus, ukuran blok, jenis cek. |

### Lihat juga

* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [XzArchive](../)
* ruang nama [Aspose.Zip.Xz](../../xzarchive/)
* perakitan [Aspose.Zip](../../../)

---

## XzArchive(Stream) {#constructor_1}

Menginisialisasi instance baru dari[`XzArchive`](../) kelas disiapkan untuk dekompresi.

```csharp
public XzArchive(Stream source)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| source | Stream | Sumber arsip. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | *source* tidak dapat dicari. |
| ArgumentNullException | *source* adalah nol. |

### Perkataan

Konstruktor ini tidak melakukan dekompresi. Melihat[`Extract`](../extract/) metode dekompresi.

### Lihat juga

* class [XzArchive](../)
* ruang nama [Aspose.Zip.Xz](../../xzarchive/)
* perakitan [Aspose.Zip](../../../)

---

## XzArchive(string) {#constructor_2}

Menginisialisasi instance baru dari[`XzArchive`](../) kelas disiapkan untuk dekompresi.

```csharp
public XzArchive(string path)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Path ke sumber arsip. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *path* adalah nol. |
| SecurityException | Penelepon tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | Itu*path* kosong, hanya berisi spasi putih, atau berisi karakter yang tidak valid. |
| UnauthorizedAccessException | Akses ke file*path* ditolak. |
| PathTooLongException | Yang ditentukan*path*, nama file, atau keduanya melebihi panjang maksimum yang ditentukan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di*path* berisi titik dua (:) di tengah string. |

### Perkataan

Konstruktor ini tidak melakukan dekompresi. Melihat[`Extract`](../extract/) metode dekompresi.

### Lihat juga

* class [XzArchive](../)
* ruang nama [Aspose.Zip.Xz](../../xzarchive/)
* perakitan [Aspose.Zip](../../../)


