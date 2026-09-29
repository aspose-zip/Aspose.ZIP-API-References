---
title: "CabEntrySettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan yang mengontrol bagaimana entri CAB ditulis."
type: docs
weight: 47
url: /id/java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

Pengaturan yang mengontrol bagaimana entri CAB ditulis.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | Menginisialisasi pengaturan dengan profil kompresi tertentu. |
| [CabEntrySettings()](#CabEntrySettings--) | Menginisialisasi pengaturan dengan kompresi MSZip default. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Mendapatkan konfigurasi kompresi yang diterapkan pada entri. |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


Menginisialisasi pengaturan dengan profil kompresi tertentu.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | Pengaturan kompresi yang akan digunakan. |

Dapat berupa salah satu dari berikut: |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


Menginisialisasi pengaturan dengan kompresi MSZip default.

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


Mendapatkan konfigurasi kompresi yang diterapkan pada entri.

Dapat menjadi salah satu dari berikut:

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
