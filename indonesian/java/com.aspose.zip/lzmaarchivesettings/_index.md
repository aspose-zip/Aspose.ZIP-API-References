---
title: "LzmaArchiveSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk arsip lzma."
type: docs
weight: 87
url: /id/java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

Pengaturan untuk arsip lzma.

Algoritma Lempel\u2013Ziv\u2013Markov chain (LZMA) adalah algoritma yang digunakan untuk melakukan kompresi data tanpa kehilangan. Algoritma ini menggunakan skema kompresi kamus yang agak mirip dengan algoritma LZ77 dan memiliki rasio kompresi tinggi serta ukuran kamus kompresi yang variabel.

Lihat selengkapnya: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | Menginisialisasi instance baru dari kelas [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) dengan ukuran kamus default, yaitu 16 megabyte, jumlah byte cepat sebesar 32, dan bit konteks literal sebesar 3. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Mendapatkan peristiwa yang dipicu ketika sebagian aliran mentah dikompresi. |
| [getDictionarySize()](#getDictionarySize--) | Ukuran kamus (buffer riwayat) menunjukkan berapa byte data tidak terkompresi yang baru saja diproses yang disimpan dalam memori. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Mendapatkan jumlah bit konteks literal. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Mendapatkan jumlah byte yang digunakan untuk pencarian kecocokan cepat dalam algoritma LZMA. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Mengatur peristiwa yang dipicu ketika sebagian aliran mentah dikompresi. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | Ukuran kamus (buffer riwayat) menunjukkan berapa byte data tidak terkompresi yang baru saja diproses yang disimpan dalam memori. |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | Mengatur jumlah bit konteks literal. |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | Mengatur jumlah byte yang digunakan untuk pencarian kecocokan cepat dalam algoritma LZMA. |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


Menginisialisasi instance baru dari kelas [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) dengan ukuran kamus default, yaitu 16 megabyte, jumlah byte cepat sebesar 32, dan bit konteks literal sebesar 3.

```

``````

LzmaArchiveSettings settings = new LzmaArchiveSettings();
settings.setDictionarySize(1048576);
try (LzmaArchive archive = new LzmaArchive(settings)) {
archive.setSource("data.bin");
archive.save(lzmaFile);
}
 
```



### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Gets an event that is raised when a portion of raw stream compressed.

```

``````

    lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Ukuran kamus (buffer riwayat) menunjukkan berapa byte data tidak terkompresi yang baru saja diproses yang disimpan dalam memori. Jika tidak diatur, akan dipilih sesuai dengan ukuran entri.

Semakin besar kamus, biasanya rasio kompresi semakin baik - tetapi kamus yang lebih besar dari data tidak terkompresi merupakan pemborosan RAM. Ukuran kamus arsip LZMA harus berupa pangkat dua (2^n) atau tiga kali pangkat dua (3\*2^n).

**Returns:**
int - Ukuran kamus (buffer riwayat).
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Mendapatkan jumlah bit konteks literal.

Bit Konteks Literal mendefinisikan berapa banyak bit paling signifikan dari byte tidak terkompresi sebelumnya yang digunakan untuk memprediksi bit dari byte literal berikutnya. Harus antara 0 hingga 8.

**Returns:**
int - jumlah bit konteks literal.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Mendapatkan jumlah byte yang digunakan untuk pencarian kecocokan cepat dalam algoritma LZMA.

Nilai yang lebih tinggi memungkinkan kompresor mencari kecocokan yang lebih panjang, yang dapat sedikit meningkatkan rasio kompresi tetapi memperlambat proses kompresi.

**Returns:**
int - jumlah byte yang digunakan untuk pencarian kecocokan cepat dalam algoritma LZMA.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Mengatur peristiwa yang dipicu ketika sebagian aliran mentah dikompresi.

```

``````

lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

### setDictionarySize(int value) {#setDictionarySize-int-}
```
public final void setDictionarySize(int value)
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. If not set, will be chosen accordingly to entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM. The disctionary size of LZMA archive must be either a power of two (2^n) or three times a power of two (3\*2^n).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Dictionary (history buffer) size. |

### setLiteralContextBits(int value) {#setLiteralContextBits-int-}
```
public final void setLiteralContextBits(int value)
```


Sets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of literal context bits. |

### setNumberOfFastBytes(int value) {#setNumberOfFastBytes-int-}
```
public final void setNumberOfFastBytes(int value)
```


Sets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of bytes used for fast match searching in the LZMA algorithm. |

