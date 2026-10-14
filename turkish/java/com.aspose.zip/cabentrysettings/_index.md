---
title: "CabEntrySettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "CAB girdisinin nasıl yazıldığını kontrol eden ayarlar."
type: docs
weight: 47
url: /tr/java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

CAB girdisinin nasıl yazıldığını kontrol eden ayarlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | Belirli bir sıkıştırma profiliyle ayarları başlatır. |
| [CabEntrySettings()](#CabEntrySettings--) | Varsayılan MSZip sıkıştırmasıyla ayarları başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Girişe uygulanan sıkıştırma yapılandırmasını alır. |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


Belirli bir sıkıştırma profiliyle ayarları başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | Kullanılacak sıkıştırma ayarları. |

Şunlardan biri olabilir: |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


Varsayılan MSZip sıkıştırmasıyla ayarları başlatır.

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


Girişe uygulanan sıkıştırma yapılandırmasını alır.

Bunlardan biri olabilir:

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
