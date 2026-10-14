---
title: "CancellationFlag"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Bendera yang memungkinkan pembatalan operasi."
type: docs
weight: 54
url: /id/java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

Bendera yang memungkinkan pembatalan operasi.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | Membuat instance CancellationFlag. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [cancel()](#cancel--) | Membatalkan operasi yang terkait dengan instance [CancellationFlag](../../com.aspose.zip/cancellationflag) ini. |
| [cancelAfter(long delay)](#cancelAfter-long-) | Membatalkan operasi setelah penundaan tertentu dalam milidetik. |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | Membatalkan operasi setelah penundaan tertentu dalam satuan waktu yang diberikan. |
| [close()](#close--) | Menutup instance [CancellationFlag](../../com.aspose.zip/cancellationflag) dan melepaskan semua sumber daya yang terkait dengannya. |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


Membuat instance CancellationFlag.

### cancel() {#cancel--}
```
public void cancel()
```


Membatalkan operasi yang terkait dengan instance [CancellationFlag](../../com.aspose.zip/cancellationflag) ini.

Jika operasi sudah dibatalkan, metode ini tidak melakukan apa-apa.

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


Membatalkan operasi setelah penundaan tertentu dalam milidetik.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| delay | long | Penundaan dalam milidetik setelah itu operasi akan dibatalkan. |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


Membatalkan operasi setelah penundaan tertentu dalam satuan waktu yang diberikan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| delay | long | Penundaan setelah itu operasi akan dibatalkan. |
| unit | java.util.concurrent.TimeUnit | Satuan waktu dari parameter penundaan. |

### close() {#close--}
```
public void close()
```


Menutup instance [CancellationFlag](../../com.aspose.zip/cancellationflag) dan melepaskan semua sumber daya yang terkait dengannya.

