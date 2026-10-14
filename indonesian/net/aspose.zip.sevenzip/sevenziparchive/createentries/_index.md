---
title: "SevenZipArchive.CreateEntries"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode SevenZipArchive. Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan"
type: docs
weight: 40
url: /id/net/aspose.zip.sevenzip/sevenziparchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```csharp
public SevenZipArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| directory | DirectoryInfo | Direktori yang akan dikompresi. |
| includeRootDirectory | Boolean | Menunjukkan apakah menyertakan direktori akar itu sendiri atau tidak. |

### Nilai Kembalian

Arsip dengan entri yang telah disusun.

### Pengecualian

| exception | kondisi |
| --- | --- |
| DirectoryNotFoundException | Jalur ke *directory* tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses *directory*. |

## Contoh

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.7z");
}
```

### Lihat Juga

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```csharp
public SevenZipArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceDirectory | String | Direktori yang akan dikompresi. |
| includeRootDirectory | Boolean | Menunjukkan apakah menyertakan direktori akar itu sendiri atau tidak. |

### Nilai Kembalian

Arsip dengan entri yang telah disusun.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentNullException | *sourceDirectory* adalah `null`. |

## Contoh

Buat arsip 7z dengan kompresi LZMA2.

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.7z");
}
```

### Lihat Juga

* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


