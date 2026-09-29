---
title: "PPMdCompressionSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración para la compresión PPMd dentro de un archivo ZIP."
type: docs
weight: 93
url: /es/java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

Configuración para la compresión PPMd dentro de un archivo ZIP.

PPMd es un algoritmo de compresión de datos desarrollado por Dmitry Shkarin. Este algoritmo se basa en la coincidencia predictiva de frases en múltiples contextos de orden.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | Inicializa una nueva instancia de la clase [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings). |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | Inicializa una nueva instancia de la clase [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) con el orden de modelo predeterminado y el tamaño del subasignador. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | Obtiene el orden del modelo. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Obtiene el tamaño del subasignador en MB. |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


Inicializa una nueva instancia de la clase [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings).

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

El orden de modelo predeterminado es 8, y el tamaño del subasignador es 50 MB.

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


Obtiene el orden del modelo.

**Returns:**
int - el orden del modelo
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Obtiene el tamaño del subasignador en MB.

**Returns:**
int - el tamaño del subasignador en MB
