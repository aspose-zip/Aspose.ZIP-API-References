---
title: "SplitArchiveSaveOptions.SplitArchiveSaveOptions"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor SplitArchiveSaveOptions. Menginisialisasi pengaturan untuk menyimpan arsip ZIP multivolume."
type: docs
weight: 10
url: /id/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions(string, uint) {#constructor}

Membuat instance pengaturan untuk menyimpan arsip ZIP multi-volume.

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | String | Nama untuk volume. Bisa dengan atau tanpa ekstensi .zip. |
| segmentSize | UInt32 | Ukuran sebuah volume. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | Ukuran segmen kurang dari 65536 byte. |

## Catatan

Beberapa volume mungkin lebih kecil dari *segmentSize*. Dalam kebanyakan kasus, segmen terakhir akan lebih kecil tetapi jarang segmen reguler mungkin terlalu kecil.

Nama file akan menjadi sebagai berikut: *fileName*.z01, *fileName*.z02, ..., *fileName*.z(n-1), *fileName*.zip.

### Lihat Juga

* class [SplitArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)

---

## SplitArchiveSaveOptions(uint) {#constructor_1}

Membuat instance pengaturan untuk menyimpan arsip ZIP multi-volume.

```csharp
public SplitArchiveSaveOptions(uint segmentSize)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| segmentSize | UInt32 | Ukuran sebuah volume. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | Ukuran segmen kurang dari 65536 byte. |

## Catatan

Gunakan instance `SplitArchiveSaveOptions` ini tanpa nama file dengan metode [`SaveSplit`](../../../aspose.zip/archive/savesplit/).

Beberapa volume mungkin lebih kecil dari *segmentSize*. Dalam kebanyakan kasus, segmen terakhir akan lebih kecil tetapi jarang segmen reguler mungkin terlalu kecil.

### Lihat Juga

* class [SplitArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


