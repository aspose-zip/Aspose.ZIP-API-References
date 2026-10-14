---
title: "AppleArchive.AppleArchive"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor AppleArchive. Menginisialisasi instance baru dari kelas AppleArchive dengan pengaturan yang digunakan untuk entri yang disusun"
type: docs
weight: 10
url: /id/net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

Menginisialisasi instance baru dari kelas [`AppleArchive`](../) dengan pengaturan yang digunakan untuk entri yang disusun.

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | Pengaturan yang digunakan saat menyusun Apple Archive baru. |

### Lihat Juga

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

Menginisialisasi instance baru dari kelas [`AppleArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |
| loadOptions | AppleArchiveLoadOptions | Opsi untuk memuat arsip yang ada. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *sourceStream* bernilai null. |
| ArgumentException | *sourceStream* tidak dapat dipindahkan. |
| InvalidDataException | *sourceStream* bukan Apple Archive yang valid. |
| EndOfStreamException | Aliran berakhir secara tak terduga selama parsing entri arsip. |

## Catatan

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [`ExtractToDirectory`](../extracttodirectory/) dan [`Open`](../../applearchiveentry/open/) untuk dekompresi.

### Lihat Juga

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

Menginisialisasi instance baru dari kelas [`AppleArchive`](../) dan menyusun daftar entri yang dapat diekstrak dari arsip.

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur lengkap atau relatif ke file arsip. |
| loadOptions | AppleArchiveLoadOptions | Opsi untuk memuat arsip yang ada. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| FileNotFoundException | Berkas tidak ditemukan. |
| InvalidDataException | *path* bukan Apple Archive yang valid. |
| EndOfStreamException | Aliran berakhir secara tak terduga selama parsing entri arsip. |

## Catatan

Konstruktor ini tidak mendekompresi entri apa pun. Lihat metode [`ExtractToDirectory`](../extracttodirectory/) dan [`Open`](../../applearchiveentry/open/) untuk dekompresi.

### Lihat Juga

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


