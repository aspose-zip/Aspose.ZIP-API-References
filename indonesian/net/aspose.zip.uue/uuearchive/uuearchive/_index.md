---
title: "UueArchive.UueArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "UueArchive konstruktor. Menginisialisasi instance baru dari kelas UueArchive yang disiapkan untuk pengkodean"
type: docs
weight: 10
url: /id/net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

Menginisialisasi instance baru dari kelas [`UueArchive`](../) yang disiapkan untuk pengkodean.

```csharp
public UueArchive()
```

## Contoh

Contoh berikut menunjukkan cara uuencode file.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### Lihat Juga

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

Menginisialisasi instance baru dari kelas [`UueArchive`](../) yang disiapkan untuk dekripsi.

```csharp
public UueArchive(Stream sourceStream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |

## Catatan

Konstruktor ini tidak melakukan dekripsi. Lihat metode [`Open`](../open/) untuk dekompresi.

## Contoh

Buka arsip dari stream dan ekstrak ke `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### Lihat Juga

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

Menginisialisasi instance baru dari kelas [`UueArchive`](../).

```csharp
public UueArchive(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke berkas arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| FileNotFoundException | Berkas tidak ditemukan. |
| IOException | Berkas sudah terbuka. |

## Catatan

Konstruktor ini tidak melakukan dekompresi. Lihat metode [`Open`](../open/) untuk dekompresi.

## Contoh

Buka arsip dari file dengan jalur dan dekode ke `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### Lihat Juga

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


