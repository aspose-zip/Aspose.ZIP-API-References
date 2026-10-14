---
title: "SevenZipArchive.Save"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode SevenZipArchive. Menyimpan arsip 7z ke aliran yang diberikan."
type: docs
weight: 80
url: /id/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream, SevenZipArchiveSaveOptions) {#save}

Menyimpan arsip 7z ke aliran yang disediakan.

```csharp
public void Save(Stream output, SevenZipArchiveSaveOptions saveOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |
| saveOptions | SevenZipArchiveSaveOptions | Opsi untuk penyimpanan arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *output* tidak mendukung pencarian. |
| ArgumentNullException | *output* adalah null. |
| InvalidOperationException | Encoder gagal mengompresi data. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |

## Catatan

*output* must be seekable.

## Contoh

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
    using (var archive = new SevenZipArchive())
    {
      archive.CreateEntry("data", source);
      archive.Save(sevenZipFile);
    }
  }
}
```

### Lihat Juga

* class [SevenZipArchiveSaveOptions](../../../aspose.zip.saving/sevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, SevenZipArchiveSaveOptions) {#save_1}

Menyimpan arsip ke file tujuan yang disediakan.

```csharp
public void Save(string destinationFileName, SevenZipArchiveSaveOptions saveOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationFileName | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |
| saveOptions | SevenZipArchiveSaveOptions | Opsi untuk penyimpanan arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *destinationFileName* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *destinationFileName* kosong, hanya berisi spasi, atau mengandung karakter tidak valid. |
| UnauthorizedAccessException | Akses ke file *destinationFileName* ditolak. |
| PathTooLongException | *destinationFileName* yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | File di *destinationFileName* berisi tanda titik dua (:) di tengah string. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| EndOfStreamException | Dilemparkan ketika akhir aliran tercapai sebelum jumlah byte yang diharapkan dibaca. |
| InvalidOperationException | Encoder gagal mengompresi data. |

## Catatan

Dimungkinkan untuk menyimpan arsip ke jalur yang sama dengan tempat ia dimuat. Namun, ini tidak disarankan karena pendekatan ini menggunakan penyalinan ke file sementara.

## Contoh

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
   using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
   {
      archive.CreateEntry("data", source);
      archive.Save("archive.7z");
   }
}
```

### Lihat Juga

* class [SevenZipArchiveSaveOptions](../../../aspose.zip.saving/sevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


