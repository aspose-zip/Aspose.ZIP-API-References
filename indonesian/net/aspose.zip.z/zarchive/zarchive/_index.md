---
title: ZArchive.ZArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: ZArchive konstruktor. Menginisialisasi instance baru dariZArchive kelas disiapkan untuk mengompresi.
type: docs
weight: 10
url: /id/net/aspose.zip.z/zarchive/zarchive/
---
## ZArchive() {#constructor}

Menginisialisasi instance baru dari[`ZArchive`](../) kelas disiapkan untuk mengompresi.

```csharp
public ZArchive()
```

### Lihat juga

* class [ZArchive](../)
* ruang nama [Aspose.Zip.Z](../../zarchive/)
* perakitan [Aspose.Zip](../../../)

---

## ZArchive(Stream) {#constructor_1}

Menginisialisasi instance baru dari[`ZArchive`](../) kelas disiapkan untuk dekompresi.

```csharp
public ZArchive(Stream source)
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

* class [ZArchive](../)
* ruang nama [Aspose.Zip.Z](../../zarchive/)
* perakitan [Aspose.Zip](../../../)

---

## ZArchive(string) {#constructor_2}

Menginisialisasi instance baru dari[`ZArchive`](../) kelas disiapkan untuk dekompresi.

```csharp
public ZArchive(string path)
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

* class [ZArchive](../)
* ruang nama [Aspose.Zip.Z](../../zarchive/)
* perakitan [Aspose.Zip](../../../)


