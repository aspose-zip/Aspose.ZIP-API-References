---
title: "Archive.DeleteEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode Archive. Menghapus kemunculan pertama entri spesifik dari daftar entri."
type: docs
weight: 70
url: /id/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

Menghapus kemunculan pertama dari entri spesifik dari daftar entri.

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| entri | ArchiveEntry | Entri yang akan dihapus dari daftar entri. |

### Nilai Kembalian

Arsip dengan entri yang dihapus.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang. |
| InvalidOperationException | Dilemparkan ketika penghapusan entri tidak valid karena keadaan arsip saat ini. |

## Contoh

Berikut cara Anda dapat menghapus semua entri kecuali yang terakhir:

```csharp
using (var archive = new Archive("archive.zip"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save("last_entry.zip");
}
```

### Lihat Juga

* class [ArchiveEntry](../../archiveentry/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Menghapus entri dari daftar entri berdasarkan indeks.

```csharp
public Archive DeleteEntry(int entryIndex)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| entryIndex | Int32 | Indeks berbasis nol dari entri yang akan dihapus. |

### Nilai Kembalian

Arsip dengan entri yang dihapus.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Archive telah dibuang. |
| ArgumentOutOfRangeException | *entryIndex* kurang dari 0.-atau- *entryIndex* sama dengan atau lebih besar dari jumlah `Entries` count. |
| InvalidOperationException | Dilemparkan ketika penghapusan entri tidak valid karena keadaan arsip saat ini. |

## Contoh

```csharp
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### Lihat Juga

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


