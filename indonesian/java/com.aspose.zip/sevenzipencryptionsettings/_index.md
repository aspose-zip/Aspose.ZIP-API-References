---
title: "SevenZipEncryptionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas dasar untuk pengaturan beberapa metode enkripsi 7z."
type: docs
weight: 112
url: /id/java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

Kelas dasar untuk pengaturan beberapa metode enkripsi 7z.

AES-256 adalah satu-satunya metode enkripsi yang memungkinkan untuk arsip 7z. Jadi [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) adalah satu-satunya implementasi.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getEncryptHeader()](#getEncryptHeader--) | Mendapatkan nilai yang menunjukkan enkripsi header. |
| [getPassword()](#getPassword--) | Mendapatkan kata sandi untuk enkripsi atau dekripsi. |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | Mengatur nilai yang menunjukkan enkripsi header. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Mengatur kata sandi untuk enkripsi atau dekripsi. |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


Mendapatkan nilai yang menunjukkan enkripsi header.

Pengaturan ini setara dengan saklar `-mhe=on` pada alat 7-Zip. Saat ini, pengaturan ini tidak kompatibel dengan kompresi header.

**Returns:**
boolean - nilai yang menunjukkan enkripsi header
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Mendapatkan kata sandi untuk enkripsi atau dekripsi.

**Returns:**
java.lang.String - kata sandi untuk enkripsi atau dekripsi
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


Mengatur nilai yang menunjukkan enkripsi header.

Pengaturan ini setara dengan saklar `-mhe=on` pada alat 7-Zip. Saat ini, pengaturan ini tidak kompatibel dengan kompresi header.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan enkripsi header |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Mengatur kata sandi untuk enkripsi atau dekripsi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | kata sandi untuk enkripsi atau dekripsi |

