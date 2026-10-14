---
title: "LzmaArchiveSettings.DictionarySize"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti LzmaArchiveSettings. Ukuran buffer riwayat kamus menunjukkan berapa byte data tidak terkompresi yang baru-baru ini diproses disimpan dalam memori. Jika tidak diatur, akan dipilih sesuai dengan ukuran entri"
type: docs
weight: 20
url: /id/net/aspose.zip.lzma/lzmaarchivesettings/dictionarysize/
---
## LzmaArchiveSettings.DictionarySize property

Ukuran kamus (buffer riwayat) menunjukkan berapa byte data tidak terkompresi yang baru-baru ini diproses yang disimpan dalam memori. Jika tidak disetel, akan dipilih sesuai dengan ukuran entri.

```csharp
public int DictionarySize { get; set; }
```

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | Nilai terlalu kecil atau terlalu besar. |
| ArgumentException | Nilai bukan pangkat dua atau tiga kali pangkat dua. |

## Catatan

Semakin besar kamus, biasanya rasio kompresi semakin baik - tetapi kamus yang lebih besar daripada data tidak terkompresi merupakan pemborosan RAM.

Ukuran kamus arsip LZMA harus berupa pangkat dua (2^n) atau tiga kali pangkat dua (3*2^n).

### Lihat Juga

* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


