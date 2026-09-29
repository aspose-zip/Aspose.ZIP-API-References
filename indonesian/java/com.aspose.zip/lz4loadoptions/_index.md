---
title: "Lz4LoadOptions"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Opsi untuk memuat ."
type: docs
weight: 82
url: /id/java/com.aspose.zip/lz4loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class Lz4LoadOptions
```

Opsi untuk memuat [Lz4Archive](../../com.aspose.zip/lz4archive).
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Lz4LoadOptions()](#Lz4LoadOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Mengatur flag pembatalan yang digunakan untuk membatalkan operasi ekstraksi. |
### Lz4LoadOptions() {#Lz4LoadOptions--}
```
public Lz4LoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Mengatur flag pembatalan yang digunakan untuk membatalkan operasi ekstraksi.

Batalkan ekstraksi arsip lz4 setelah waktu tertentu.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
Lz4LoadOptions options = new Lz4LoadOptions();
options.setCancellationFlag(cf);
try (Lz4Archive a = new Lz4Archive("big.lz4", options)) {
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

