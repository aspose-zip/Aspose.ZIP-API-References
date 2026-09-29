---
title: "SevenZipCipher"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas dasar untuk sifir AES yang digunakan untuk enkripsi 7-zip."
type: docs
weight: 110
url: /id/java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

Kelas dasar untuk sifir AES yang digunakan untuk enkripsi 7-zip.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | Mengambil nilai yang menunjukkan apakah transformasi saat ini dapat digunakan kembali. |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | Mengambil nilai yang menunjukkan apakah beberapa blok dapat ditransformasikan. |
| [dispose()](#dispose--) | Melakukan tugas yang ditentukan aplikasi yang terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola. |
| [getInputBlockSize()](#getInputBlockSize--) | Mengambil ukuran blok input. |
| [getOutputBlockSize()](#getOutputBlockSize--) | Mengambil ukuran blok output. |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | Mengubah wilayah yang ditentukan dari array byte input dan menyalin transformasi yang dihasilkan ke wilayah yang ditentukan dari array byte output. |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | Mengubah wilayah yang ditentukan dari array byte yang ditentukan. |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


Mengambil nilai yang menunjukkan apakah transformasi saat ini dapat digunakan kembali.

**Returns:**
boolean - nilai yang menunjukkan apakah transformasi saat ini dapat digunakan kembali
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


Mengambil nilai yang menunjukkan apakah beberapa blok dapat ditransformasikan.

**Returns:**
boolean - nilai yang menunjukkan apakah beberapa blok dapat ditransformasikan
### dispose() {#dispose--}
```
public abstract void dispose()
```


Melakukan tugas yang ditentukan aplikasi yang terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola.

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


Mengambil ukuran blok input.

**Returns:**
int - ukuran blok input
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


Mengambil ukuran blok output.

**Returns:**
int - ukuran blok output
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


Mengubah wilayah yang ditentukan dari array byte input dan menyalin transformasi yang dihasilkan ke wilayah yang ditentukan dari array byte output.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| inputBuffer | byte[] | input untuk menghitung transformasi |
| inputOffset | int | offset ke dalam array byte input dari mana mulai menggunakan data |
| inputCount | int | jumlah byte dalam array byte input yang akan digunakan sebagai data |
| outputBuffer | byte[] | output yang akan ditulisi transformasi |
| outputOffset | int | offset ke dalam array byte output dari mana mulai menulis data |

**Returns:**
int - jumlah byte yang ditulis
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


Mengubah wilayah yang ditentukan dari array byte yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| inputBuffer | byte[] | input untuk menghitung transformasi |
| inputOffset | int | offset ke dalam array byte input dari mana mulai menggunakan data |
| inputCount | int | jumlah byte dalam array byte input yang akan digunakan sebagai data |

**Returns:**
byte[] - transformasi yang dihitung
