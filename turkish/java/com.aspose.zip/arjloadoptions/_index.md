---
title: "ArjLoadOptions"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Sıkıştırılmış bir dosyadan arşivin yüklendiği seçenekler."
type: docs
weight: 39
url: /tr/java/com.aspose.zip/arjloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArjLoadOptions
```

Sıkıştırılmış bir dosyadan arşivin yüklendiği seçenekler.

.NET Framework 4.0 ve üzeri sürümlerde, çıkarma işlemini iptal etmek için kullanılabilir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ArjLoadOptions()](#ArjLoadOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Çıkarma işlemini iptal etmek için kullanılan bir iptal bayrağı ayarlar. |
### ArjLoadOptions() {#ArjLoadOptions--}
```
public ArjLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Çıkarma işlemini iptal etmek için kullanılan bir iptal bayrağı ayarlar.

Belirli bir süreden sonra ARJ arşivi çıkartmayı iptal et.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
ArjLoadOptions options = new ArjLoadOptions();
options.setCancellationFlag(cf);
try (ArjArchive a = new ArjArchive(\"big.arj\", options)) {
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

