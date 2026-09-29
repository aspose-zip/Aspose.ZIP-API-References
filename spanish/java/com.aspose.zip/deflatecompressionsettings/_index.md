---
title: "DeflateCompressionSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración para la compresión Deflate dentro de un archivo ZIP."
type: docs
weight: 59
url: /es/java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

Configuración para la compresión Deflate dentro de un archivo ZIP.

Deflate es un algoritmo de compresión de datos sin pérdida que utiliza una combinación del algoritmo LZ77 y la codificación Huffman.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | Inicializa una nueva instancia de la clase [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings). |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


Inicializa una nueva instancia de la clase [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



