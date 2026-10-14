---
title: "DeflateCompressionSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки сжатия Deflate внутри ZIP‑архива."
type: docs
weight: 59
url: /ru/java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

Настройки сжатия Deflate внутри ZIP‑архива.

Deflate — это алгоритм без потерь сжатия данных, использующий комбинацию алгоритма LZ77 и кодирования Хаффмана.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | Инициализирует новый экземпляр класса [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings). |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


Инициализирует новый экземпляр класса [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



