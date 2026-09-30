---
title: "TarArchive.SaveXzCompressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode TarArchive. Menyimpan arsip ke aliran dengan kompresi xz"
type: docs
weight: 200
url: /id/net/aspose.zip.tar/tararchive/savexzcompressed/
---
## SaveXzCompressed(Stream, TarFormat?, XzArchiveSettings) {#savexzcompressed}

Menyimpan arsip ke aliran dengan kompresi xz.

```csharp
public void SaveXzCompressed(Stream output, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |
| format | Nullable`1 | Mendefinisikan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan. |
| pengaturan | XzArchiveSettings | Kumpulan pengaturan arsip xz tertentu: ukuran kamus, ukuran blok, tipe pemeriksaan. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *output* adalah null. |
| ArgumentException | *output* tidak dapat ditulis. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan |
| IOException | Terjadi kesalahan I/O. |

## Catatan

*output*The stream must be writable.

## Contoh

```csharp
using (FileStream result = File.OpenWrite("result.tar.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### Lihat Juga

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, TarFormat?, XzArchiveSettings) {#savexzcompressed_1}

Menyimpan arsip ke jalur berdasarkan jalur dengan kompresi xz.

```csharp
public void SaveXzCompressed(string path, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |
| format | Nullable`1 | Mendefinisikan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan. |
| pengaturan | XzArchiveSettings | Kumpulan pengaturan arsip xz tertentu: ukuran kamus, ukuran blok, tipe pemeriksaan. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| UnauthorizedAccessException | Pemanggil tidak memiliki izin yang diperlukan. -atau- *path* menunjukkan file atau direktori hanya-baca. |
| ArgumentException | *path* adalah string dengan panjang nol, hanya berisi spasi, atau berisi satu atau lebih karakter tidak valid sebagaimana didefinisikan oleh InvalidPathChars. |
| ArgumentNullException | *path* bernilai null. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| DirectoryNotFoundException | *path* yang ditentukan tidak valid, (misalnya, berada pada drive yang tidak dipetakan). |
| NotSupportedException | *path* berada dalam format yang tidak valid. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan |
| IOException | Terjadi kesalahan I/O. |

## Contoh

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.tar.xz");
    }
}
```

### Lihat Juga

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


