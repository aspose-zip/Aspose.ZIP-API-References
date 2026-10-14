---
title: "PPMdCompressionSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "ZIP arşivi içinde PPMd sıkıştırması için ayarlar."
type: docs
weight: 93
url: /tr/java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

ZIP arşivi içinde PPMd sıkıştırması için ayarlar.

PPMd, Dmitry Shkarin tarafından geliştirilen bir veri sıkıştırma algoritmasıdır. Bu algoritma, birden çok sıra bağlamında öngörücü ifade eşleştirmesine dayanır.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | Yeni bir [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) sınıfının örneğini başlatır. |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | Varsayılan model sırası ve alt‑ayırıcı boyutu ile yeni bir [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) sınıfının örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | Modelin sırasını alır. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Alt-ayırıcı boyutunu MB cinsinden alır. |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


Yeni bir [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) sınıfının örneğini başlatır.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10)))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| modelOrder | int | Order of the model.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### PPMdCompressionSettings() {#PPMdCompressionSettings--}
```
public PPMdCompressionSettings()
```


Initializes a new instance of the [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) class with default model order and sub-allocator size.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("zipFile.zip");
     }
 
```

Varsayılan model sırası 8'dir ve alt‑ayırıcı boyutu 50 MB'dir.

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


Modelin sırasını alır.

**Returns:**
int - modelin sırası
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Alt-ayırıcı boyutunu MB cinsinden alır.

**Returns:**
int - alt-ayırıcı boyutu MB cinsinden
