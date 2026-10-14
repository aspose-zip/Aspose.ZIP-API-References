---
title: "XzCompressionSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки сжатия Xz внутри ZIP-архива."
type: docs
weight: 149
url: /ru/java/com.aspose.zip/xzcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class XzCompressionSettings extends CompressionSettings
```

Настройки сжатия Xz внутри ZIP-архива.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [XzCompressionSettings()](#XzCompressionSettings--) | Инициализирует новый экземпляр класса [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings). |
### XzCompressionSettings() {#XzCompressionSettings--}
```
public XzCompressionSettings()
```


Инициализирует новый экземпляр класса [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save("archive.zip");
}
 
```



