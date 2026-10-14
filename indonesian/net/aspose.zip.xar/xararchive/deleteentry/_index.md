---
title: "XarArchive.DeleteEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode XarArchive. Menghapus kemunculan pertama dari entri tertentu dari daftar entri."
type: docs
weight: 50
url: /id/net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

Menghapus kemunculan pertama dari entri tertentu dalam daftar entri.

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| entri | XarEntry | Entri yang akan dihapus dari daftar entri. |

### Nilai Kembalian

Instansi entri Xar.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *entry* bernilai null. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| InvalidOperationException | Arsip tidak dibuka untuk ekstraksi. |

## Contoh

Berikut cara Anda dapat menghapus semua entri kecuali yang terakhir:

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### Lihat Juga

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


