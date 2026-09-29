---
title: "CabLoadOptions"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Opsi dengan mana arsip dimuat dari file terkompresi."
type: docs
weight: 48
url: /id/java/com.aspose.zip/cabloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class CabLoadOptions
```

Opsi dengan mana arsip dimuat dari file terkompresi.

Mengizinkan pembatalan ekstraksi untuk .NET Framework 4.0 ke atas.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [CabLoadOptions()](#CabLoadOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Mengatur flag pembatalan yang digunakan untuk membatalkan operasi ekstraksi. |
### CabLoadOptions() {#CabLoadOptions--}
```
public CabLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Mengatur flag pembatalan yang digunakan untuk membatalkan operasi ekstraksi.

Batalkan ekstraksi arsip CAB setelah waktu tertentu.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
CabLoadOptions options = new CabLoadOptions();
options.setCancellationFlag(cf);
try (CabArchive a = new CabArchive("big.cab", options)) {
try {
a.getEntries().get(0).extract("data.bin");
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

