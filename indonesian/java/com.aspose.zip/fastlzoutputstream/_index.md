---
title: "FastLZOutputStream"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pembungkus aliran yang mengompresi data dengan FastLZ."
type: docs
weight: 68
url: /id/java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

Pembungkus aliran yang mengompresi data dengan FastLZ. Menerapkan pola dekorator.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | Menginisialisasi instance baru dari kelas FastLZStream yang disiapkan untuk kompresi. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [close()](#close--) | Menutup aliran saat ini dan melepaskan semua sumber daya (seperti soket dan pegangan file) yang terkait dengan aliran saat ini. |
| [flush()](#flush--) | Mengosongkan semua buffer untuk aliran ini dan menyebabkan data yang di-buffer ditulis ke perangkat dasar. |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | Menulis urutan byte ke aliran kompresi dan memajukan posisi saat ini dalam aliran ini sebanyak jumlah byte yang ditulis. |
| [write(int b)](#write-int-) | Menulis byte yang ditentukan ke aliran keluaran ini. |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


Menginisialisasi instance baru dari kelas FastLZStream yang disiapkan untuk kompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | java.io.OutputStream | aliran untuk menyimpan data terkompresi |
| compressionLevel | int | gunakan 1 untuk kompresi lebih cepat, gunakan 2 untuk rasio kompresi yang lebih baik |

### close() {#close--}
```
public void close()
```


Menutup aliran saat ini dan melepaskan semua sumber daya (seperti soket dan pegangan file) yang terkait dengan aliran saat ini.

### flush() {#flush--}
```
public void flush()
```


Mengosongkan semua buffer untuk aliran ini dan menyebabkan data yang di-buffer ditulis ke perangkat dasar.

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


Menulis urutan byte ke aliran kompresi dan memajukan posisi saat ini dalam aliran ini sebanyak jumlah byte yang ditulis.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| buffer | byte[] | sebuah array byte. Metode ini menyalin count byte dari buffer ke aliran saat ini |
| offset | int | offset byte berbasis nol dalam buffer di mana penyalinan byte ke aliran saat ini dimulai |
| count | int | jumlah byte yang akan ditulis ke aliran saat ini |

### write(int b) {#write-int-}
```
public void write(int b)
```


Menulis byte yang ditentukan ke aliran keluaran ini. Kontrak umum untuk `write` adalah satu byte ditulis ke aliran keluaran. Byte yang akan ditulis adalah delapan bit urutan rendah dari argumen `b`. 24 bit urutan tinggi dari `b` diabaikan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| b | int | byte `byte` |

