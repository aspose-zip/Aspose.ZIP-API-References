---
title: SharArchive.DeleteEntry
second_title: Aspose.ZIP untuk Referensi .NET API
description: SharArchive metode. Menghapus kejadian pertama dari entri tertentu dari daftar entri.
type: docs
weight: 50
url: /id/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

Menghapus kejadian pertama dari entri tertentu dari daftar entri.

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| entry | SharEntry | Entri untuk dihapus dari daftar entri. |

### Nilai Pengembalian

Contoh entri Shar.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *entry* adalah nol. |

### Contoh

Inilah cara Anda dapat menghapus semua entri kecuali yang terakhir:

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### Lihat juga

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* ruang nama [Aspose.Zip.Shar](../../shararchive/)
* perakitan [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Menghapus entri dari daftar entri menurut indeks.

```csharp
public SharArchive DeleteEntry(int entryIndex)
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
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### Lihat juga

* class [SharArchive](../)
* ruang nama [Aspose.Zip.Shar](../../shararchive/)
* perakitan [Aspose.Zip](../../../)


