---
title: "Lz4ArchiveSetting"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk komposisi arsip LZ4."
type: docs
weight: 81
url: /id/java/com.aspose.zip/lz4archivesetting/
---

**Inheritance:**
java.lang.Object
```
public class Lz4ArchiveSetting
```

Pengaturan untuk komposisi arsip LZ4.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Lz4ArchiveSetting()](#Lz4ArchiveSetting--) | Menginisialisasi instance baru dari [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) dengan parameter default. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getIncludeBlockChecksum()](#getIncludeBlockChecksum--) | Mendapatkan nilai yang menunjukkan apakah menyertakan hash xxh32 terkompresi di akhir blok terkompresi. |
| [getIncludeContentChecksum()](#getIncludeContentChecksum--) | Mendapatkan nilai yang menunjukkan apakah menyertakan hash xxh32 konten di akhir arsip LZ4. |
| [getIncludeContentSize()](#getIncludeContentSize--) | Mendapatkan nilai yang menunjukkan apakah menyertakan ukuran konten dalam frame. |
| [setIncludeBlockChecksum(boolean value)](#setIncludeBlockChecksum-boolean-) | Mengatur nilai yang menunjukkan apakah menyertakan hash xxh32 terkompresi di akhir blok terkompresi. |
| [setIncludeContentChecksum(boolean value)](#setIncludeContentChecksum-boolean-) | Mengatur nilai yang menunjukkan apakah menyertakan hash xxh32 konten di akhir arsip LZ4. |
| [setIncludeContentSize(boolean value)](#setIncludeContentSize-boolean-) | Mengatur nilai yang menunjukkan apakah menyertakan ukuran konten dalam frame. |
### Lz4ArchiveSetting() {#Lz4ArchiveSetting--}
```
public Lz4ArchiveSetting()
```


Menginisialisasi instance baru dari [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) dengan parameter default.

### getIncludeBlockChecksum() {#getIncludeBlockChecksum--}
```
public final boolean getIncludeBlockChecksum()
```


Mendapatkan nilai yang menunjukkan apakah menyertakan hash xxh32 terkompresi di akhir blok terkompresi.

Default adalah false.

**Returns:**
boolean - nilai yang menunjukkan apakah menyertakan hash xxh32 terkompresi di akhir blok terkompresi.
### getIncludeContentChecksum() {#getIncludeContentChecksum--}
```
public final boolean getIncludeContentChecksum()
```


Mendapatkan nilai yang menunjukkan apakah menyertakan hash xxh32 konten di akhir arsip LZ4.

Default adalah true.

**Returns:**
boolean - nilai yang menunjukkan apakah akan menyertakan hash xxh32 konten di akhir arsip LZ4.
### getIncludeContentSize() {#getIncludeContentSize--}
```
public final boolean getIncludeContentSize()
```


Mendapatkan nilai yang menunjukkan apakah menyertakan ukuran konten dalam frame.

Defaultnya adalah false. Diterapkan ketika aliran sumber dapat dicari.

**Returns:**
boolean - nilai yang menunjukkan apakah akan menyertakan ukuran konten dalam frame.
### setIncludeBlockChecksum(boolean value) {#setIncludeBlockChecksum-boolean-}
```
public final void setIncludeBlockChecksum(boolean value)
```


Mengatur nilai yang menunjukkan apakah menyertakan hash xxh32 terkompresi di akhir blok terkompresi.

Default adalah false.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan menyertakan hash xxh32 terkompresi di akhir blok terkompresi. |

### setIncludeContentChecksum(boolean value) {#setIncludeContentChecksum-boolean-}
```
public final void setIncludeContentChecksum(boolean value)
```


Mengatur nilai yang menunjukkan apakah menyertakan hash xxh32 konten di akhir arsip LZ4.

Default adalah true.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan menyertakan hash xxh32 konten di akhir arsip LZ4. |

### setIncludeContentSize(boolean value) {#setIncludeContentSize-boolean-}
```
public final void setIncludeContentSize(boolean value)
```


Mengatur nilai yang menunjukkan apakah menyertakan ukuran konten dalam frame.

Defaultnya adalah false. Diterapkan ketika aliran sumber dapat dicari.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan menyertakan ukuran konten dalam frame. |

