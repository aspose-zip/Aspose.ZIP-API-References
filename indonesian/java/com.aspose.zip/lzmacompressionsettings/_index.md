---
title: "LzmaCompressionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk metode kompresi LZMA."
type: docs
weight: 88
url: /id/java/com.aspose.zip/lzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class LzmaCompressionSettings extends CompressionSettings
```

Pengaturan untuk metode kompresi LZMA.

Algoritma Lempel\u2013Ziv\u2013Markov chain (LZMA) adalah algoritma yang digunakan untuk melakukan kompresi data tanpa kehilangan. Algoritma ini menggunakan skema kompresi kamus yang agak mirip dengan algoritma LZ77 dan memiliki rasio kompresi tinggi serta ukuran kamus kompresi yang variabel.

Lihat selengkapnya: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [LzmaCompressionSettings()](#LzmaCompressionSettings--) | Menginisialisasi instance baru dari kelas [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) dengan parameter default. |
| [LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#LzmaCompressionSettings-int-int-int-) | Menginisialisasi instance baru dari kelas [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) dengan ukuran kamus yang ditentukan, jumlah fast byte, dan jumlah bit konteks literal. |
| [LzmaCompressionSettings(int dictionarySize)](#LzmaCompressionSettings-int-) | Menginisialisasi instance baru dari kelas [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) dengan ukuran kamus yang ditentukan, jumlah fast byte default sebesar 32, dan jumlah bit konteks literal sebesar 3. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | Ukuran kamus (buffer riwayat) menunjukkan berapa byte data tidak terkompresi yang baru saja diproses yang disimpan dalam memori. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Mendapatkan jumlah bit konteks literal. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Mendapatkan jumlah byte yang digunakan untuk pencarian kecocokan cepat dalam algoritma LZMA. |
### LzmaCompressionSettings() {#LzmaCompressionSettings--}
```
public LzmaCompressionSettings()
```


Menginisialisasi instance baru dari kelas [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) dengan parameter default.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



### LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits) {#LzmaCompressionSettings-int-int-int-}
```
public LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)
```


Initializes a new instance of the [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) class with specified dictionary size, number of fast bytes and number of literal context bits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824. |
| numberOfFastBytes | int | The number of bytes used for fast match searching in the LZMA algorithm. Can be in the range from 5 to 273. |
| literalContextBits | int | Sets the number of literal context bits (high bits of previous literal). It can be in range from 0 to 8. |

### LzmaCompressionSettings(int dictionarySize) {#LzmaCompressionSettings-int-}
```
public LzmaCompressionSettings(int dictionarySize)
```


Initializes a new instance of the [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) class with specified dictionary size, default number of fast bytes equal to 32 and number of literal context bits equal to 3.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824. |

### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

**Returns:**
int - how many bytes of the recently processed uncompressed data are kept in memory.
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Gets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Returns:**
int - the number of literal context bits.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Gets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Returns:**
int - the number of bytes used for fast match searching in the LZMA algorithm.
