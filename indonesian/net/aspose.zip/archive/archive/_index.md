---
title: Archive.Archive
second_title: Aspose.ZIP untuk Referensi .NET API
description: Archive konstruktor. Menginisialisasi instance baru dariArchive kelas dengan pengaturan opsional untuk entrientrinya.
type: docs
weight: 10
url: /id/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

Menginisialisasi instance baru dari[`Archive`](../) kelas dengan pengaturan opsional untuk entri-entrinya.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | Pengaturan kompresi dan enkripsi digunakan untuk yang baru ditambahkan[`ArchiveEntry`](../../archiveentry/) items. Jika tidak ditentukan, kompresi Deflate paling umum tanpa enkripsi akan digunakan. |

### Contoh

Contoh berikut menunjukkan cara mengompres satu file dengan pengaturan default.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### Lihat juga

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* ruang nama [Aspose.Zip](../../archive/)
* perakitan [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

Menginisialisasi instance baru dari[`Archive`](../) kelas dan menulis daftar entri dapat diekstraksi dari arsip.

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |
| loadOptions | ArchiveLoadOptions | Opsi untuk memuat arsip yang ada. |
| newEntrySettings | ArchiveEntrySettings | Pengaturan kompresi dan enkripsi digunakan untuk yang baru ditambahkan[`ArchiveEntry`](../../archiveentry/) items. Jika tidak ditentukan, kompresi Deflate paling umum tanpa enkripsi akan digunakan. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | *sourceStream* tidak dapat dicari. |
| InvalidDataException | Header enkripsi untuk AES bertentangan dengan metode kompresi WinZip. |

### Perkataan

Konstruktor ini tidak mendekompres entri apa pun. Melihat[`Open`](../../archiveentry/open/) metode dekompresi.

### Contoh

Contoh berikut mengekstrak arsip terenkripsi, lalu mendekompres entri pertama ke a`MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Lihat juga

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* ruang nama [Aspose.Zip](../../archive/)
* perakitan [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

Menginisialisasi instance baru dari[`Archive`](../) kelas dan menulis daftar entri dapat diekstraksi dari arsip.

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Jalur yang sepenuhnya memenuhi syarat atau relatif ke file arsip. |
| loadOptions | ArchiveLoadOptions | Opsi untuk memuat arsip yang ada. |
| newEntrySettings | ArchiveEntrySettings | Pengaturan kompresi dan enkripsi digunakan untuk yang baru ditambahkan[`ArchiveEntry`](../../archiveentry/) items. Jika tidak ditentukan, kompresi Deflate paling umum tanpa enkripsi akan digunakan. |

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

Konstruktor ini tidak mendekompres entri apa pun. Melihat[`Open`](../../archiveentry/open/) metode dekompresi.

### Contoh

Contoh berikut mengekstrak arsip terenkripsi, lalu mendekompres entri pertama ke a`MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Lihat juga

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* ruang nama [Aspose.Zip](../../archive/)
* perakitan [Aspose.Zip](../../../)


