---
title: "XzBcjX86FilterSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración del filtro xz Bcj X86."
type: docs
weight: 148
url: /es/java/com.aspose.zip/xzbcjx86filtersettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XzFilterSettings](../../com.aspose.zip/xzfiltersettings)
```
public final class XzBcjX86FilterSettings extends XzFilterSettings
```

Configuración del filtro xz Bcj X86.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [XzBcjX86FilterSettings()](#XzBcjX86FilterSettings--) | Inicializa una nueva instancia de la [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). |
### XzBcjX86FilterSettings() {#XzBcjX86FilterSettings--}
```
public XzBcjX86FilterSettings()
```


Inicializa una nueva instancia de la [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). Úsela para comprimir archivos ejecutables y bibliotecas dentro de [XzArchive](../../com.aspose.zip/xzarchive).

```

``````

XzLZMA2FilterSettings lzma2 = new XzLZMA2FilterSettings(5242880);
XzBcjX86FilterSettings bcj = new XzBcjX86FilterSettings();
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {bcj,lzma2}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource(\"data.bin\");
archive.save("archive.xz");
}
 
```



