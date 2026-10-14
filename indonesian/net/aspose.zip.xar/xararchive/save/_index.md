---
title: "XarArchive.Save"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode XarArchive. Menyimpan arsip ke file tujuan yang diberikan."
type: docs
weight: 80
url: /id/net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

Menyimpan arsip ke file tujuan yang disediakan.

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationFileName | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |
| saveOptions | XarSaveOptions | Opsi untuk menyimpan arsip xar. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *destinationFileName* bernilai null. |
| InvalidOperationException | Tidak dapat memodifikasi arsip xar. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| IOException | Terjadi kesalahan I/O saat membuka file. |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. |
| UnauthorizedAccessException | *destinationFileName* menunjukkan sebuah file yang hanya-baca. -atau- *destinationFileName* menunjukkan sebuah direktori. -atau- Pemanggil tidak memiliki izin yang diperlukan. |

### Lihat Juga

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

Menyimpan arsip ke aliran yang disediakan.

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |
| saveOptions | XarSaveOptions | Opsi untuk menyimpan arsip xar. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *output* adalah null. |
| ArgumentException | *output* tidak dapat ditulis/dibaca atau tidak dapat di-seek. |
| InvalidOperationException | Tidak dapat memodifikasi arsip xar. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

### Lihat Juga

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


