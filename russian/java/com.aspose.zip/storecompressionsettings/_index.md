---
title: "StoreCompressionSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки сжатия Store в архиве ZIP."
type: docs
weight: 124
url: /ru/java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

Настройки сжатия Store в архиве ZIP.

Этот метод сохраняет оригинальные данные в их исходном виде.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | Инициализирует новый экземпляр класса [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings). |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


Инициализирует новый экземпляр класса [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



