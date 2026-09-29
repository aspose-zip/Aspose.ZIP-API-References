---
title: "GzipLoadOptions"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Opsi untuk memuat ."
type: docs
weight: 70
url: /id/java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

Opsi untuk memuat [GzipArchive](../../com.aspose.zip/gziparchive).

Pada .NET Framework 4.0 ke atas, dapat digunakan untuk membatalkan ekstraksi.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | Mendapatkan nilai yang menunjukkan apakah harus mengurai header aliran untuk menentukan properti, termasuk nama. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Mengatur flag pembatalan yang digunakan untuk membatalkan operasi ekstraksi. |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | Mengatur nilai yang menunjukkan apakah harus mengurai header aliran untuk menentukan properti, termasuk nama. |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


Mendapatkan nilai yang menunjukkan apakah harus mengurai header aliran untuk menentukan properti, termasuk nama. Hanya masuk akal untuk aliran yang dapat dicari.

**Returns:**
boolean - nilai yang menunjukkan apakah harus mengurai header aliran untuk menentukan properti, termasuk nama.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Mengatur flag pembatalan yang digunakan untuk membatalkan operasi ekstraksi.

Batalkan ekstraksi arsip gzip setelah waktu tertentu.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
GzipLoadOptions options = new GzipLoadOptions();
options.setCancellationFlag(cf);
try (GzipArchive a = new GzipArchive("big.gz", options)) {
try {
a.extract("data.bin");
} catch (OperationCanceledException e) {
System.out.println("Ekstraksi dibatalkan setelah 60 detik");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

### setParseHeader(boolean value) {#setParseHeader-boolean-}
```
public final void setParseHeader(boolean value)
```


Sets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | the value indicating whether to parse stream header to figure out properties, including name. |

