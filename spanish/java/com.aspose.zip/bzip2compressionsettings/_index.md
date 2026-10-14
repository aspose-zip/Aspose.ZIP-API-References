---
title: "Bzip2CompressionSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración para la compresión Bzip2 dentro de un archivo ZIP."
type: docs
weight: 41
url: /es/java/com.aspose.zip/bzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class Bzip2CompressionSettings extends CompressionSettings
```

Configuración para la compresión Bzip2 dentro de un archivo ZIP.

bzip2 comprime archivos usando el algoritmo de compresión de texto por ordenación de bloques Burrows-Wheeler y codificación Huffman.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Bzip2CompressionSettings(int blockSize)](#Bzip2CompressionSettings-int-) | Inicializa una nueva instancia de la clase [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings). |
| [Bzip2CompressionSettings()](#Bzip2CompressionSettings--) | Inicializa una nueva instancia de la clase [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) con el tamaño de bloque predeterminado, equivalente a 9 cientos de kilobytes. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Tamaño de bloque en cientos de kilobytes. |
### Bzip2CompressionSettings(int blockSize) {#Bzip2CompressionSettings-int-}
```
public Bzip2CompressionSettings(int blockSize)
```


Inicializa una nueva instancia de la clase [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1)))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | Block size in hundreds of kilobytes. |

### Bzip2CompressionSettings() {#Bzip2CompressionSettings--}
```
public Bzip2CompressionSettings()
```


Initializes a new instance of the [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save(zipFile);
     }
 
```



### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Tamaño de bloque en cientos de kilobytes.

**Returns:**
int - tamaño de bloque en cientos de kilobytes
