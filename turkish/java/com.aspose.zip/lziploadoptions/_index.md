---
title: "LzipLoadOptions"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Yükleme seçenekleri."
type: docs
weight: 85
url: /tr/java/com.aspose.zip/lziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LzipLoadOptions
```

Yükleme seçenekleri [LzipArchive](../../com.aspose.zip/lziparchive).

.NET Framework 4.0 ve üzeri sürümlerde, çıkarma işlemini iptal etmek için kullanılabilir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LzipLoadOptions()](#LzipLoadOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Çıkarma işlemini iptal etmek için kullanılan bir iptal bayrağı ayarlar. |
### LzipLoadOptions() {#LzipLoadOptions--}
```
public LzipLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Çıkarma işlemini iptal etmek için kullanılan bir iptal bayrağı ayarlar.

Belirli bir süreden sonra lzip arşivi çıkarmayı iptal et.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LzipLoadOptions options = new LzipLoadOptions();
options.setCancellationFlag(cf);
try (LzipArchive a = new LzipArchive("big.lz", options)) {
try {
a.extract("data.bin");
} catch (OperationCanceledException e) {
System.out.println("Çıkarma 60 saniye sonra iptal edildi");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

