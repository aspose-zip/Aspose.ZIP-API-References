---
title: "GzipLoadOptions"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Yükleme seçenekleri."
type: docs
weight: 70
url: /tr/java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

Yükleme seçenekleri [GzipArchive](../../com.aspose.zip/gziparchive).

.NET Framework 4.0 ve üzeri sürümlerde, çıkarma işlemini iptal etmek için kullanılabilir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | Akış başlığını ayrıştırarak özellikleri, adı da dahil olmak üzere, belirlemek için değeri alır. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Çıkarma işlemini iptal etmek için kullanılan bir iptal bayrağı ayarlar. |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | Akış başlığını ayrıştırarak özellikleri, adı da dahil olmak üzere, belirlemek için değeri ayarlar. |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


Akış başlığını ayrıştırarak özellikleri (adı dahil) belirlemek için değeri alır. Yalnızca aranabilir akışlar için anlamlıdır.

**Returns:**
boolean - akış başlığını ayrıştırarak özellikleri, adı da dahil olmak üzere, belirlemek için değeri.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Çıkarma işlemini iptal etmek için kullanılan bir iptal bayrağı ayarlar.

Belirli bir süreden sonra gzip arşivi çıkarma işlemini iptal edin.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
GzipLoadOptions options = new GzipLoadOptions();
options.setCancellationFlag(cf);
try (GzipArchive a = new GzipArchive("big.gz", options)) {
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

### setParseHeader(boolean value) {#setParseHeader-boolean-}
```
public final void setParseHeader(boolean value)
```


Sets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | the value indicating whether to parse stream header to figure out properties, including name. |

