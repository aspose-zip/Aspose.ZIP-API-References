---
title: "CpioArchive.DeleteEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "CpioArchive metode. Menghapus kemunculan pertama dari entri spesifik dari daftar entri"
type: docs
weight: 50
url: /id/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

Menghapus kemunculan pertama dari entri tertentu dalam daftar entri.

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| entri | CpioEntry | Entri yang akan dihapus dari daftar entri. |

### Nilai Kembalian

Instansi entri Cpio.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *entry* bernilai null. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

Berikut cara Anda dapat menghapus semua entri kecuali yang terakhir:

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### Lihat Juga

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Menghapus entri dari daftar entri berdasarkan indeks.

```csharp
public CpioArchive DeleteEntry(int entryIndex)
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

## Contoh

```csharp
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### Lihat Juga

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


