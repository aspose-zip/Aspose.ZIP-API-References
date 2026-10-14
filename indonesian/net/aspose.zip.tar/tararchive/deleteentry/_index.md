---
title: "TarArchive.DeleteEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode TarArchive. Menghapus kemunculan pertama dari entri tertentu dalam daftar entri"
type: docs
weight: 120
url: /id/net/aspose.zip.tar/tararchive/deleteentry/
---
## DeleteEntry(TarEntry) {#deleteentry}

Menghapus kemunculan pertama dari entri tertentu dalam daftar entri.

```csharp
public TarArchive DeleteEntry(TarEntry entry)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| entri | TarEntry | Entri yang akan dihapus dari daftar entri. |

### Nilai Kembalian

Arsip dengan entri yang dihapus.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan |

## Contoh

Berikut cara Anda dapat menghapus semua entri kecuali yang terakhir:

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputTarFile);
}
```

### Lihat Juga

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Menghapus entri dari daftar entri berdasarkan indeks.

```csharp
public TarArchive DeleteEntry(int entryIndex)
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
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan |

## Contoh

```csharp
using (var archive = new TarArchive("two_files.tar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.tar");
}
```

### Lihat Juga

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


