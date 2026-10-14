---
title: "Kelas SevenZipLZMACompressionSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.Saving.SevenZipLZMACompressionSettings. Pengaturan untuk metode kompresi LMA dalam arsip 7z"
type: docs
weight: 1090
url: /id/net/aspose.zip.saving/sevenziplzmacompressionsettings/
---
## SevenZipLZMACompressionSettings class

Pengaturan untuk metode kompresi LZMA dalam arsip 7z.

```csharp
public class SevenZipLZMACompressionSettings : SevenZipCompressionSettings
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/#constructor)() | Menginisialisasi instance baru dari kelas `SevenZipLZMACompressionSettings` dengan parameter default. |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/#constructor_1)(int) | Menginisialisasi instance baru dari kelas `SevenZipLZMACompressionSettings` dengan ukuran kamus yang ditentukan, jumlah fast bytes sebesar 32, dan jumlah literal context bits sebesar 3. |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/#constructor_2)(int, int, int) | Menginisialisasi instance baru dari kelas `SevenZipLZMACompressionSettings` dengan ukuran kamus yang ditentukan, jumlah fast bytes, dan jumlah literal context bits. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [DictionarySize](../../aspose.zip.saving/sevenziplzmacompressionsettings/dictionarysize/) { get; set; } | Ukuran kamus (buffer riwayat) menunjukkan berapa byte data tidak terkompresi yang baru saja diproses yang disimpan dalam memori. Jika tidak disetel, akan dipilih sesuai dengan ukuran entri. Harus berada di antara 4096 dan 1073741824, atau sama dengan nol untuk deteksi otomatis berdasarkan ukuran entri. |
| [LiteralContextBits](../../aspose.zip.saving/sevenziplzmacompressionsettings/literalcontextbits/) { get; } | Mendapatkan jumlah bit konteks literal. |
| override [Method](../../aspose.zip.saving/sevenziplzmacompressionsettings/method/) { get; } | Mendapatkan metode kompresi atau dekompresi. |
| [NumberOfFastBytes](../../aspose.zip.saving/sevenziplzmacompressionsettings/numberoffastbytes/) { get; } | Mendapatkan jumlah byte yang digunakan untuk pencarian kecocokan cepat dalam algoritma LZMA. |

## Catatan

Algoritma Lempel–Ziv–Markov chain (LZMA) adalah algoritma yang digunakan untuk melakukan kompresi data tanpa kehilangan. Algoritma ini menggunakan skema kompresi kamus yang agak mirip dengan algoritma LZ77 dan memiliki rasio kompresi tinggi serta ukuran kamus kompresi yang dapat diubah.

Lihat selengkapnya: [Lempel–Ziv–Markov chain algorithm](https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm)

### Lihat Juga

* class [SevenZipCompressionSettings](../sevenzipcompressionsettings/)
* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


