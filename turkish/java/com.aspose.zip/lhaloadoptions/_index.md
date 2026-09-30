---
title: "LhaLoadOptions"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Sıkıştırılmış bir dosyadan arşivin yüklendiği seçenekler."
type: docs
weight: 78
url: /tr/java/com.aspose.zip/lhaloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LhaLoadOptions
```

Sıkıştırılmış bir dosyadan arşivin yüklendiği seçenekler.

.NET Framework 4.0 ve üzeri sürümlerde, çıkarma işlemini iptal etmek için kullanılabilir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LhaLoadOptions()](#LhaLoadOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Çıkarma işlemini iptal etmek için kullanılan bir iptal bayrağı ayarlar. |
### LhaLoadOptions() {#LhaLoadOptions--}
```
public LhaLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Çıkarma işlemini iptal etmek için kullanılan bir iptal bayrağı ayarlar.

Belirli bir süreden sonra LHA arşivi çıkarma işlemini iptal edin.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LhaLoadOptions options = new LhaLoadOptions();
options.setCancellationFlag(cf);
try (LhaArchive a = new LhaArchive("big.lha", options)) {
try {
a.getEntries().get(0).extract(\"data.bin\");
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

