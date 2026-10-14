---
title: "ProgressCancelEventArgs"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Kelas untuk data acara yang dapat dibatalkan yang berisi jumlah byte yang diproses."
type: docs
weight: 95
url: /id/java/com.aspose.zip/progresscanceleventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.ProgressEventArgs](../../com.aspose.zip/progresseventargs)
```
public class ProgressCancelEventArgs extends ProgressEventArgs
```

Kelas untuk data acara yang dapat dibatalkan yang berisi jumlah byte yang diproses.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ProgressCancelEventArgs(long proceededBytes)](#ProgressCancelEventArgs-long-) | Menginisialisasi sebuah instance baru dari kelas [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCancel()](#getCancel--) | Mendapatkan nilai yang menunjukkan apakah acara harus dibatalkan. |
| [setCancel(boolean value)](#setCancel-boolean-) | Mengatur nilai yang menunjukkan apakah acara harus dibatalkan. |
### ProgressCancelEventArgs(long proceededBytes) {#ProgressCancelEventArgs-long-}
```
public ProgressCancelEventArgs(long proceededBytes)
```


Menginisialisasi sebuah instance baru dari kelas [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| proceededBytes | long | Jumlah byte yang diproses. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Mendapatkan nilai yang menunjukkan apakah acara harus dibatalkan.

**Returns:**
boolean - True jika peristiwa harus dibatalkan; jika tidak, false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Mengatur nilai yang menunjukkan apakah acara harus dibatalkan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah peristiwa harus dibatalkan. |

