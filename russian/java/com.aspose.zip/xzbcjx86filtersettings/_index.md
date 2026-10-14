---
title: "XzBcjX86FilterSettings"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Настройки фильтра xz Bcj X86."
type: docs
weight: 148
url: /ru/java/com.aspose.zip/xzbcjx86filtersettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XzFilterSettings](../../com.aspose.zip/xzfiltersettings)
```
public final class XzBcjX86FilterSettings extends XzFilterSettings
```

Настройки фильтра xz Bcj X86.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [XzBcjX86FilterSettings()](#XzBcjX86FilterSettings--) | Инициализирует новый экземпляр [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). |
### XzBcjX86FilterSettings() {#XzBcjX86FilterSettings--}
```
public XzBcjX86FilterSettings()
```


Инициализирует новый экземпляр [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). Используйте его для сжатия исполняемых файлов и библиотек внутри [XzArchive](../../com.aspose.zip/xzarchive).

```

``````

XzLZMA2FilterSettings lzma2 = new XzLZMA2FilterSettings(5242880);
XzBcjX86FilterSettings bcj = new XzBcjX86FilterSettings();
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {bcj,lzma2}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource("data.bin");
archive.save("archive.xz");
}
 
```



