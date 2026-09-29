---
title: "ArjLoadOptions"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Opsi dengan mana arsip dimuat dari file terkompresi."
type: docs
weight: 39
url: /id/java/com.aspose.zip/arjloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArjLoadOptions
```

Opsi dengan mana arsip dimuat dari file terkompresi.

Pada .NET Framework 4.0 ke atas, dapat digunakan untuk membatalkan ekstraksi.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ArjLoadOptions()](#ArjLoadOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Mengatur flag pembatalan yang digunakan untuk membatalkan operasi ekstraksi. |
### ArjLoadOptions() {#ArjLoadOptions--}
```
public ArjLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Mengatur flag pembatalan yang digunakan untuk membatalkan operasi ekstraksi.

Batalkan ekstraksi arsip ARJ setelah waktu tertentu.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
ArjLoadOptions options = new ArjLoadOptions();
options.setCancellationFlag(cf);
try (ArjArchive a = new ArjArchive("big.arj", options)) {
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

