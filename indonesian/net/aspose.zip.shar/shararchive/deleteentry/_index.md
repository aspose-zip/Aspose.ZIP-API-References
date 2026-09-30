---
title: "SharArchive.DeleteEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode SharArchive. Menghapus kemunculan pertama dari entri spesifik dari daftar entri"
type: docs
weight: 50
url: /id/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

Menghapus kemunculan pertama dari entri tertentu dalam daftar entri.

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| entri | SharEntry | Entri yang akan dihapus dari daftar entri. |

### Nilai Kembalian

Instance entri Shar.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *entry* bernilai null. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| InvalidOperationException | Arsip ini dibuka untuk ekstraksi. |

## Contoh

Berikut cara Anda dapat menghapus semua entri kecuali yang terakhir:

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### Lihat Juga

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Menghapus entri dari daftar entri berdasarkan indeks.

```csharp
public SharArchive DeleteEntry(int entryIndex)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| entryIndex | Int32 | Indeks berbasis nol dari entri yang akan dihapus. |

### Nilai Kembalian

Arsip dengan entri yang dihapus.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* kurang dari 0.-atau- *entryIndex* sama dengan atau lebih besar dari jumlah `Entries` count. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| InvalidOperationException | Arsip ini dibuka untuk ekstraksi. |

## Contoh

```csharp
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### Lihat Juga

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


