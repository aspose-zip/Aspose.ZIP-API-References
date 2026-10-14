---
title: "StoreCompressionSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración de la compresión Store dentro de un archivo ZIP."
type: docs
weight: 124
url: /es/java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

Configuración de la compresión Store dentro de un archivo ZIP.

Este método almacena los datos originales tal como están.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | Inicializa una nueva instancia de la clase [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings). |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


Inicializa una nueva instancia de la clase [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



