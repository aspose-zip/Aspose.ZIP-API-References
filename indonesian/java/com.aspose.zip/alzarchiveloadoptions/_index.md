---
title: "AlzArchiveLoadOptions"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Opsi yang digunakan untuk memuat arsip ALZ dari file terkompresi."
type: docs
weight: 12
url: /id/java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

Opsi yang digunakan untuk memuat arsip ALZ dari file terkompresi.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Mendapatkan kata sandi yang digunakan untuk mendekripsi entri. |
| [getEncoding()](#getEncoding--) | Mendapatkan enkoding yang digunakan untuk nama entri. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | Mendapatkan apakah verifikasi checksum dari entri ALZ dilewati. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Mengatur flag pembatalan yang digunakan untuk membatalkan ekstraksi. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Mengatur kata sandi yang digunakan untuk mendekripsi entri. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Mengatur enkoding yang digunakan untuk nama entri. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | Mengatur apakah verifikasi checksum dari entri ALZ dilewati. |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


Mendapatkan kata sandi yang digunakan untuk mendekripsi entri.

**Returns:**
java.lang.String - kata sandi yang digunakan untuk mendekripsi entri, atau `null` ketika tidak ada yang dikonfigurasi
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Mendapatkan enkoding yang digunakan untuk nama entri. Defaultnya adalah halaman kode Windows Korea 949 (CP949). Arsip ALZ secara historis menyimpan nama file menggunakan halaman kode ANSI Windows Korea.

**Returns:**
java.nio.charset.Charset - enkoding yang digunakan untuk nama entri
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


Mendapatkan apakah verifikasi checksum dari entri ALZ dilewati. Defaultnya adalah `false`.

**Returns:**
boolean - apakah verifikasi checksum dilewati
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Mengatur flag pembatalan yang digunakan untuk membatalkan ekstraksi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | flag pembatalan, atau `null` untuk menonaktifkan pembatalan |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


Mengatur kata sandi yang digunakan untuk mendekripsi entri.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | kata sandi yang digunakan untuk mendekripsi entri |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Mengatur enkoding yang digunakan untuk nama entri. Arsip ALZ secara historis menyimpan nama file menggunakan halaman kode ANSI Windows Korea.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.nio.charset.Charset | enkoding yang digunakan untuk nama entri |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


Mengatur apakah verifikasi checksum dari entri ALZ dilewati.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | apakah verifikasi checksum dilewati |

