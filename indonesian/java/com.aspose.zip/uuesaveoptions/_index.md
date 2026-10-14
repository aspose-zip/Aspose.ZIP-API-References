---
title: "UueSaveOptions"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Opsi untuk menyimpan file yang di-uuencode."
type: docs
weight: 129
url: /id/java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

Opsi untuk menyimpan file yang di-uuencode.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | Menginisialisasi opsi dengan nama file yang diberikan pengguna dan baris baru. |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | Menginisialisasi opsi dengan nama file yang diberikan pengguna dan baris baru default. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getFileName()](#getFileName--) | Mendapatkan nama file yang akan digunakan saat membuat kembali data yang terdekripsi. |
| [getNewLine()](#getNewLine--) | Mendapatkan karakter yang mengakhiri setiap baris, biasanya "\n" atau "\r\n". |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | Mendapatkan izin file Unix file tersebut. |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | Mengatur izin file Unix. |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


Menginisialisasi opsi dengan nama file yang diberikan pengguna dan baris baru.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | nama file yang akan digunakan saat membuat ulang data yang didekode |
| newLine | java.lang.String | karakter yang mengakhiri setiap baris |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


Menginisialisasi opsi dengan nama file yang diberikan pengguna dan baris baru default.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileName | java.lang.String | nama file yang akan digunakan saat membuat ulang data yang didekode |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Mendapatkan nama file yang akan digunakan saat membuat kembali data yang terdekripsi.

**Returns:**
java.lang.String - nama file yang akan digunakan saat membuat ulang data yang didekode
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


Mendapatkan karakter yang mengakhiri setiap baris, biasanya "\n" atau "\r\n".

**Returns:**
java.lang.String - karakter yang mengakhiri setiap baris, biasanya "\n" atau "\r\n".
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


Mendapatkan izin file Unix file tersebut.

Default adalah 644.

**Returns:**
java.lang.String - izin Unix file.
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


Mengatur izin file Unix.

Default adalah 644.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | izin Unix file. |

