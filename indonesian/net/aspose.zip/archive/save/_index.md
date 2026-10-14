---
title: "Archive.Save"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode Archive. Menyimpan arsip ke aliran yang disediakan."
type: docs
weight: 100
url: /id/net/aspose.zip/archive/save/
---
## Save(Stream, ArchiveSaveOptions) {#save}

Menyimpan arsip ke aliran yang disediakan.

```csharp
public void Save(Stream outputStream, ArchiveSaveOptions saveOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| outputStream | Stream | Aliran tujuan. |
| saveOptions | ArchiveSaveOptions | Opsi untuk penyimpanan arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *outputStream* tidak dapat ditulis. |
| ObjectDisposedException | Arsip telah dibuang. |
| InvalidOperationException | Dilemparkan ketika enkripsi diterapkan pada entri yang sudah terenkripsi. |

## Catatan

*outputStream* must be writable.

## Contoh

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(zipFile);
    }
}
```

### Lihat Juga

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ArchiveSaveOptions) {#save_1}

Menyimpan arsip ke file tujuan yang disediakan.

```csharp
public void Save(string destinationFileName, ArchiveSaveOptions saveOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationFileName | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |
| saveOptions | ArchiveSaveOptions | Opsi untuk penyimpanan arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *destinationFileName* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *destinationFileName* kosong, hanya berisi spasi, atau mengandung karakter tidak valid. |
| UnauthorizedAccessException | Akses ke file *destinationFileName* ditolak. |
| PathTooLongException | *destinationFileName* yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| NotSupportedException | File di *destinationFileName* berisi tanda titik dua (:) di tengah string. |
| FileNotFoundException | Berkas tidak ditemukan. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| IOException | Berkas sudah terbuka. |
| ObjectDisposedException | Dilempar jika arsip telah dibuang. |
| InvalidOperationException | Dilemparkan ketika enkripsi diterapkan pada entri yang sudah terenkripsi. |

## Catatan

Dimungkinkan untuk menyimpan arsip ke jalur yang sama dengan tempat ia dimuat. Namun, ini tidak disarankan karena pendekatan ini menggunakan penyalinan ke file sementara.

## Contoh

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Lihat Juga

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


