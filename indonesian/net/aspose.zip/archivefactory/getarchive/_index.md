---
title: "ArchiveFactory.GetArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode ArchiveFactory. Mendeteksi format arsip dan membuat objek IArchive yang sesuai berdasarkan tipe arsip yang ditentukan oleh path yang diberikan"
type: docs
weight: 20
url: /id/net/aspose.zip/archivefactory/getarchive/
---
## GetArchive(string) {#getarchive_2}

Mendeteksi format arsip dan membuat objek [`IArchive`](../../iarchive/) yang sesuai berdasarkan tipe arsip yang ditentukan oleh path yang diberikan.

```csharp
public static IArchive GetArchive(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Path ke arsip yang akan dianalisis. |

### Nilai Kembalian

Objek [`IArchive`](../../iarchive/) yang merepresentasikan arsip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* adalah `null`. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, (misalnya, berada pada drive yang tidak dipetakan). |
| FileNotFoundException | File yang ditentukan dalam *path* tidak ditemukan. |
| IOException | Terjadi kesalahan I/O saat membuka file. |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. |
| UnauthorizedAccessException | *path* menunjuk ke sebuah direktori. -atau- Pemanggil tidak memiliki izin yang diperlukan. |

### Lihat Juga

* interface [IArchive](../../iarchive/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)

---

## GetArchive(Stream) {#getarchive}

Mendeteksi format arsip dan membuat objek [`IArchive`](../../iarchive/) yang sesuai berdasarkan tipe arsip yang ditentukan oleh aliran yang diberikan.

```csharp
public static IArchive GetArchive(Stream stream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran yang berisi data arsip. Aliran ini harus dapat di-seek. |

### Nilai Kembalian

Objek [`IArchive`](../../iarchive/) yang merepresentasikan arsip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *stream* tidak dapat di-seek. |
| ArgumentNullException | *stream* bernilai null. |

### Lihat Juga

* interface [IArchive](../../iarchive/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)

---

## GetArchive(Stream, string) {#getarchive_1}

Mendeteksi format arsip dan membuat objek [`IArchive`](../../iarchive/) yang sesuai berdasarkan tipe arsip terenkripsi yang ditentukan oleh aliran yang diberikan.

```csharp
public static IArchive GetArchive(Stream stream, string password)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran yang berisi data arsip. Aliran ini harus dapat di-seek. |
| password | String | Kata sandi untuk mendekripsi arsip terenkripsi. |

### Nilai Kembalian

Objek [`IArchive`](../../iarchive/) yang merepresentasikan arsip.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *stream* tidak dapat di-seek. |
| ArgumentNullException | *stream* bernilai null. |

### Lihat Juga

* interface [IArchive](../../iarchive/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


