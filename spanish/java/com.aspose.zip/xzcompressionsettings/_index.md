---
title: "XzCompressionSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración de la compresión Xz dentro de un archivo ZIP."
type: docs
weight: 149
url: /es/java/com.aspose.zip/xzcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class XzCompressionSettings extends CompressionSettings
```

Configuración de la compresión Xz dentro de un archivo ZIP.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [XzCompressionSettings()](#XzCompressionSettings--) | Inicializa una nueva instancia de la clase [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings). |
### XzCompressionSettings() {#XzCompressionSettings--}
```
public XzCompressionSettings()
```


Inicializa una nueva instancia de la clase [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(\"archive.zip\");
}
 
```



