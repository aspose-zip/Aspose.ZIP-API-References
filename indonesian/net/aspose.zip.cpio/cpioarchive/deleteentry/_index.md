---
title: CpioArchive.DeleteEntry
second_title: Aspose.ZIP untuk Referensi .NET API
description: CpioArchive metode. Menghapus kejadian pertama dari entri tertentu dari daftar entri.
type: docs
weight: 50
url: /id/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

Menghapus kejadian pertama dari entri tertentu dari daftar entri.

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| entry | CpioEntry | Entri untuk dihapus dari daftar entri. |

### Nilai Pengembalian

Contoh entri Cpio.

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *entry* adalah nol. |

### Contoh

Inilah cara Anda dapat menghapus semua entri kecuali yang terakhir:

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### Lihat juga

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* ruang nama [Aspose.Zip.Cpio](../../cpioarchive/)
* perakitan [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Menghapus entri dari daftar entri menurut indeks.

```csharp
public CpioArchive DeleteEntry(int entryIndex)
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
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### Lihat juga

* class [CpioArchive](../)
* ruang nama [Aspose.Zip.Cpio](../../cpioarchive/)
* perakitan [Aspose.Zip](../../../)


