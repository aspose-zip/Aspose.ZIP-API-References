---
title: "AppleArchive.Save"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode AppleArchive. Menyimpan arsip ke aliran yang disediakan."
type: docs
weight: 90
url: /id/net/aspose.zip.apple/applearchive/save/
---
## Save(Stream) {#save}

Menyimpan arsip ke aliran yang disediakan.

```csharp
public void Save(Stream output)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang. |
| ArgumentNullException | *output* adalah `null`. |
| ArgumentException | *output* tidak dapat ditulis. |
| ArgumentOutOfRangeException | Ukuran blok LZ4 atau Zlib yang dikonfigurasi tidak positif. |
| NotSupportedException | Pengaturan kompresi hilang atau tidak didukung, komposisi langsung menggunakan aliran yang tidak dapat di-seek, atau ukuran entri/arsip melebihi batas Apple Archive saat ini. |

## Catatan

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### Lihat Juga

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Menyimpan arsip ke file tujuan yang disediakan.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationFileName | String | Jalur arsip yang akan dibuat. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang. |
| ArgumentException | *destinationFileName* tidak valid. |
| ArgumentNullException | *destinationFileName* adalah `null`. |
| ArgumentOutOfRangeException | Ukuran blok LZ4 atau Zlib yang dikonfigurasi tidak positif. |
| NotSupportedException | Pengaturan kompresi hilang atau tidak didukung, komposisi langsung menggunakan aliran yang tidak dapat di-seek, atau ukuran entri/arsip melebihi batas Apple Archive saat ini. |

### Lihat Juga

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


