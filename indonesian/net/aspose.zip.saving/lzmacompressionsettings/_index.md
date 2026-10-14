---
title: "Kelas LzmaCompressionSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Saving.LzmaCompressionSettings. Pengaturan untuk kompresi LZMA dalam arsip ZIP"
type: docs
weight: 960
url: /id/net/aspose.zip.saving/lzmacompressionsettings/
---
## LzmaCompressionSettings class

Pengaturan untuk kompresi LZMA dalam arsip ZIP.

```csharp
public class LzmaCompressionSettings : CompressionSettings
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [LzmaCompressionSettings](lzmacompressionsettings/#constructor)() | Menginisialisasi sebuah instance baru dari kelas `LzmaCompressionSettings` dengan parameter default. |
| [LzmaCompressionSettings](lzmacompressionsettings/#constructor_1)(int) | Menginisialisasi sebuah instance baru dari kelas `LzmaCompressionSettings` dengan ukuran kamus yang ditentukan, jumlah fast bytes default sebesar 32, dan jumlah literal context bits sebesar 3. |
| [LzmaCompressionSettings](lzmacompressionsettings/#constructor_2)(int, int, int) | Menginisialisasi instance baru dari kelas `LzmaCompressionSettings` dengan ukuran kamus yang ditentukan, jumlah byte cepat, dan jumlah bit konteks literal. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [DictionarySize](../../aspose.zip.saving/lzmacompressionsettings/dictionarysize/) { get; } | Ukuran kamus (buffer riwayat) menunjukkan berapa byte data tidak terkompresi yang baru-baru ini diproses yang disimpan dalam memori. |
| [LiteralContextBits](../../aspose.zip.saving/lzmacompressionsettings/literalcontextbits/) { get; } | Mendapatkan jumlah bit konteks literal. |
| [NumberOfFastBytes](../../aspose.zip.saving/lzmacompressionsettings/numberoffastbytes/) { get; } | Mendapatkan jumlah byte yang digunakan untuk pencarian kecocokan cepat dalam algoritma LZMA. |

## Catatan

Algoritma Lempel–Ziv–Markov chain (LZMA) adalah algoritma yang digunakan untuk melakukan kompresi data tanpa kehilangan. Algoritma ini menggunakan skema kompresi kamus yang agak mirip dengan algoritma LZ77 dan memiliki rasio kompresi tinggi serta ukuran kamus kompresi yang dapat diubah.

Lihat selengkapnya: [Lempel–Ziv–Markov chain algorithm](https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm)

### Lihat Juga

* class [CompressionSettings](../compressionsettings/)
* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


