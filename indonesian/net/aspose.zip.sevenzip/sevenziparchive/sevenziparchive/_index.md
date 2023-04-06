---
title: SevenZipArchive.SevenZipArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: SevenZipArchive konstruktor. Menginisialisasi instance baru dariSevenZipArchive kelas dengan pengaturan opsional untuk entrientrinya.
type: docs
weight: 10
url: /id/net/aspose.zip.sevenzip/sevenziparchive/sevenziparchive/
---
## SevenZipArchive(SevenZipEntrySettings) {#constructor}

Menginisialisasi instance baru dari[`SevenZipArchive`](../) kelas dengan pengaturan opsional untuk entri-entrinya.

```csharp
public SevenZipArchive(SevenZipEntrySettings newEntrySettings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| newEntrySettings | SevenZipEntrySettings | Pengaturan kompresi dan enkripsi digunakan untuk yang baru ditambahkan[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) items. Jika tidak ditentukan, kompresi LZMA tanpa enkripsi akan digunakan. |

### Contoh

Contoh berikut menunjukkan cara mengompresi satu file dengan pengaturan default: Kompresi LZMA tanpa enkripsi.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Lihat juga

* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* ruang nama [Aspose.Zip.SevenZip](../../sevenziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream) {#constructor_1}

Menginisialisasi instance baru dari[`SevenZipArchive`](../) kelas dan menulis daftar entri dapat diekstraksi dari arsip.

```csharp
public SevenZipArchive(Stream sourceStream)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | *sourceStream* tidak dapat dicari. |
| ArgumentNullException | *sourceStream* adalah nol. |
| NotImplementedException | Arsip berisi lebih dari satu pembuat kode. Sekarang hanya kompresi LZMA yang didukung. |

### Perkataan

Konstruktor ini tidak mendekompres entri apa pun. Melihat[`ExtractToDirectory`](../extracttodirectory/) metode dekompresi.

### Contoh

```csharp
using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z")))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat juga

* class [SevenZipArchive](../)
* ruang nama [Aspose.Zip.SevenZip](../../sevenziparchive/)
* perakitan [Aspose.Zip](../../../)

---

## SevenZipArchive(string) {#constructor_2}

Menginisialisasi instance baru dari[`SevenZipArchive`](../) kelas dan menulis daftar entri dapat diekstraksi dari arsip.

```csharp
public SevenZipArchive(string path)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Jalur yang sepenuhnya memenuhi syarat atau relatif ke file arsip. |

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

Konstruktor ini tidak mendekompres entri apa pun. Melihat[`ExtractToDirectory`](../extracttodirectory/) metode dekompresi.

### Contoh

```csharp
using (SevenZipArchive archive = new SevenZipArchive("archive.7z"))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Lihat juga

* class [SevenZipArchive](../)
* ruang nama [Aspose.Zip.SevenZip](../../sevenziparchive/)
* perakitan [Aspose.Zip](../../../)


