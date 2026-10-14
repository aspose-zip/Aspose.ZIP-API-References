---
title: "TarArchive.SaveLZMACompressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode TarArchive. Menyimpan arsip ke aliran dengan kompresi LZMA"
type: docs
weight: 190
url: /id/net/aspose.zip.tar/tararchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, TarFormat?) {#savelzmacompressed}

Menyimpan arsip ke aliran dengan kompresi LZMA.

```csharp
public void SaveLZMACompressed(Stream output, TarFormat? format = default)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |
| format | Nullable`1 | Mendefinisikan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *output* adalah null. |
| ArgumentException | *output* tidak dapat ditulis. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan |
| IOException | Terjadi kesalahan I/O. |

## Catatan

*output* must be writable.

Penting: arsip tar disusun kemudian dikompresi dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

## Contoh

```csharp
using (FileStream result = File.OpenWrite("result.tar.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
        }
    }
}
```

### Lihat Juga

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZMACompressed(string, TarFormat?) {#savelzmacompressed_1}

Menyimpan arsip ke file berdasarkan jalur dengan kompresi lzma.

```csharp
public void SaveLZMACompressed(string path, TarFormat? format = default)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |
| format | Nullable`1 | Mendefinisikan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan. |

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

## Catatan

Penting: arsip tar disusun kemudian dikompresi dalam metode ini, isinya disimpan secara internal. Waspadai konsumsi memori.

## Contoh

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.tar.lzma");
    }
}
```

### Lihat Juga

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


