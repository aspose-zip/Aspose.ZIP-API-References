---
title: RarArchive.RarArchive
second_title: Aspose.ZIP untuk Referensi .NET API
description: RarArchive konstruktor. Menginisialisasi instance baru dariRarArchive kelas dan menulis daftar entri dapat diekstraksi dari arsip.
type: docs
weight: 10
url: /id/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

Menginisialisasi instance baru dari[`RarArchive`](../) kelas dan menulis daftar entri dapat diekstraksi dari arsip.

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Jalur yang sepenuhnya memenuhi syarat atau relatif ke file arsip. |
| loadOptions | RarArchiveLoadOptions | Opsi untuk memuat arsip yang ada. |

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

Konstruktor ini tidak mendekompres entri apa pun. Melihat[`Open`](../../rararchiveentry/open/) metode dekompresi.

### Contoh

Contoh berikut mengekstrak arsip, lalu mendekompres entri pertama ke a`MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive("data.rar"))
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

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* ruang nama [Aspose.Zip.Rar](../../rararchive/)
* perakitan [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

Menginisialisasi instance baru dari[`RarArchive`](../) kelas dan menulis daftar entri dapat diekstraksi dari arsip.

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| sourceStream | Stream | Sumber arsip. |
| loadOptions | RarArchiveLoadOptions | Opsi untuk memuat arsip yang ada. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | *sourceStream* tidak dapat dicari. |
| InvalidDataException | Tanda tangan salah untuk arsip. - atau - File tersebut bukan arsip RAR. |
| InvalidOperationException |  |

### Perkataan

Konstruktor ini tidak mendekompres entri apa pun. Melihat[`Open`](../../rararchiveentry/open/) metode dekompresi.

### Contoh

Contoh berikut menguraikan dan mendekompres entri pertama ke a`MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.rar");
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive(fs, new RarArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* ruang nama [Aspose.Zip.Rar](../../rararchive/)
* perakitan [Aspose.Zip](../../../)


