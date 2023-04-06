---
title: TarArchive.DeleteEntry
second_title: Aspose.ZIP untuk Referensi .NET API
description: TarArchive metode. Menghapus kejadian pertama dari entri tertentu dari daftar entri.
type: docs
weight: 90
url: /id/net/aspose.zip.tar/tararchive/deleteentry/
---
## DeleteEntry(TarEntry) {#deleteentry}

Menghapus kejadian pertama dari entri tertentu dari daftar entri.

```csharp
public TarArchive DeleteEntry(TarEntry entry)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| entry | TarEntry | Entri untuk dihapus dari daftar entri. |

### Nilai Pengembalian

Arsip dengan entri dihapus.

### Contoh

Inilah cara Anda dapat menghapus semua entri kecuali yang terakhir:

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputTarFile);
}
```

### Lihat juga

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* ruang nama [Aspose.Zip.Tar](../../tararchive/)
* perakitan [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Menghapus entri dari daftar entri menurut indeks.

```csharp
public TarArchive DeleteEntry(int entryIndex)
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
using (var archive = new TarArchive("two_files.tar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.tar");
}
```

### Lihat juga

* class [TarArchive](../)
* ruang nama [Aspose.Zip.Tar](../../tararchive/)
* perakitan [Aspose.Zip](../../../)


