---
title: "ZArchive.ZArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor ZArchive. Menginisialisasi sebuah instance baru dari kelas ZArchive yang disiapkan untuk kompresi"
type: docs
weight: 10
url: /id/net/aspose.zip.z/zarchive/zarchive/
---
## ZArchive() {#constructor}

Menginisialisasi sebuah instance baru dari kelas [`ZArchive`](../) yang disiapkan untuk kompresi.

```csharp
public ZArchive()
```

### Lihat Juga

* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZArchive(Stream, ZArchiveLoadOptions) {#constructor_1}

Menginisialisasi sebuah instance baru dari kelas [`ZArchive`](../) yang disiapkan untuk dekompresi.

```csharp
public ZArchive(Stream source, ZArchiveLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | Stream | Sumber arsip. |
| loadOptions | ZArchiveLoadOptions | Opsi untuk memuat arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *source* tidak dapat dicari. |
| ArgumentNullException | *source* bernilai null. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Extract`](../extract/) untuk dekompresi.

### Lihat Juga

* class [ZArchiveLoadOptions](../../zarchiveloadoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZArchive(string, ZArchiveLoadOptions) {#constructor_2}

Menginisialisasi sebuah instance baru dari kelas [`ZArchive`](../) yang disiapkan untuk dekompresi.

```csharp
public ZArchive(string path, ZArchiveLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke sumber arsip. |
| loadOptions | ZArchiveLoadOptions | Opsi untuk memuat arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| FileNotFoundException | Berkas tidak ditemukan. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| IOException | Berkas sudah terbuka. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Extract`](../extract/) untuk dekompresi.

### Lihat Juga

* class [ZArchiveLoadOptions](../../zarchiveloadoptions/)
* class [ZArchive](../)
* namespace [Aspose.Zip.Z](../../zarchive/)
* assembly [Aspose.Zip](../../../)


