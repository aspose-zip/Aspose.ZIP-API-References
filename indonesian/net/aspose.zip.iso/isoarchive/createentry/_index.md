---
title: "IsoArchive.CreateEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode IsoArchive. Menambahkan berkas ke citra ISO"
type: docs
weight: 40
url: /id/net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

Menambahkan file ke gambar ISO.

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Jalur berkas dalam ISO. |
| filePath | String | Jalur file. |

### Nilai Kembalian

Entri ISO telah disusun.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *filePath* bernilai null. |
| ArgumentException | *filePath* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke file *filePath* ditolak. |
| PathTooLongException | *filePath* yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | File di *filePath* mengandung tanda titik dua (:) di tengah string. |
| IOException | Terjadi kesalahan I/O saat membuka file. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, (misalnya, berada pada drive yang tidak dipetakan). |
| FileNotFoundException | File yang ditentukan di *filePath* tidak ditemukan. |
| InvalidOperationException | Arsip tidak berada dalam mode penyuntingan. |

### Lihat Juga

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Menambahkan file ke gambar ISO.

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Jalur berkas dalam ISO. |
| source | Stream | Aliran yang berisi data file. |

### Nilai Kembalian

Entri ISO telah disusun.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentNullException | Dilempar ketika *name* atau *source* bernilai null. |
| InvalidOperationException | Arsip tidak berada dalam mode penyuntingan. |

### Lihat Juga

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

Menambahkan file ke gambar ISO.

```csharp
public IsoEntry CreateEntry(string name)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Jalur direktori di dalam ISO. |

### Nilai Kembalian

Entri ISO telah disusun.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | `name` adalah null atau kosong. |
| InvalidOperationException | Arsip dibuka untuk ekstraksi. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

### Lihat Juga

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


