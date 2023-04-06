---
title: Archive.DeleteEntry
second_title: Aspose.ZIP untuk Referensi .NET API
description: Archive metode. Menghapus kejadian pertama dari entri tertentu dari daftar entri.
type: docs
weight: 60
url: /id/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

Menghapus kejadian pertama dari entri tertentu dari daftar entri.

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| entry | ArchiveEntry | Entri untuk dihapus dari daftar entri. |

### Nilai Pengembalian

Arsip dengan entri dihapus.

### Contoh

Inilah cara Anda dapat menghapus semua entri kecuali yang terakhir:

```csharp
using (var archive = new Archive("archive.zip"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save("last_entry.zip");
}
```

### Lihat juga

* class [ArchiveEntry](../../archiveentry/)
* class [Archive](../)
* ruang nama [Aspose.Zip](../../archive/)
* perakitan [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Menghapus entri dari daftar entri menurut indeks.

```csharp
public Archive DeleteEntry(int entryIndex)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| entryIndex | Int32 | Indeks entri berbasis nol yang akan dihapus. |

### Nilai Pengembalian

Arsip dengan entri dihapus.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* kurang dari 0,-atau-*entryIndex* sama dengan atau lebih besar dari`Entri` menghitung. |

### Contoh

```csharp
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### Lihat juga

* class [Archive](../)
* ruang nama [Aspose.Zip](../../archive/)
* perakitan [Aspose.Zip](../../../)


