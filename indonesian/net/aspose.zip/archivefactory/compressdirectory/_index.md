---
title: "ArchiveFactory.CompressDirectory"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode ArchiveFactory. Mengompres direktori yang ditentukan menjadi file arsip menggunakan format arsip yang disediakan"
type: docs
weight: 10
url: /id/net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

Mengompres direktori yang ditentukan ke dalam file arsip menggunakan format arsip yang disediakan.

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Path ke direktori yang akan dikompres. |
| outputFileName | String | Nama file tujuan. |
| archiveFormat | ArchiveFormat | Format arsip yang akan dibuat (mis., zip, rar, tar, dll.). |

### Pengecualian

| exception | kondisi |
| --- | --- |
| DirectoryNotFoundException | Dilemparkan jika direktori yang ditentukan oleh *path* tidak ada. |
| ArgumentException | Dilemparkan jika *path* bernilai null atau string kosong. |
| NotSupportedException | Dilemparkan jika *archiveFormat* yang ditentukan tidak didukung atau tidak dikenali. |
| ArgumentNullException | *path* adalah `null`. |

## Catatan

Metode ini akan membuat file arsip di lokasi yang ditentukan oleh parameter *path*. Nama file arsip biasanya akan menjadi nama direktori diikuti oleh ekstensi file yang sesuai berdasarkan *archiveFormat*. Direktori itu sendiri tidak diubah atau dihapus.

## Contoh

Berikut contoh cara menggunakan metode CompressDirectory:

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// Ini akan membuat file ZIP dengan isi direktori pada path yang ditentukan.
```

### Lihat Juga

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


