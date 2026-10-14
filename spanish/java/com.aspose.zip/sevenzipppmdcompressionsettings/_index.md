---
title: "SevenZipPPMdCompressionSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración para el método de compresión PPMd dentro de un archivo 7z."
type: docs
weight: 117
url: /es/java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

Configuración para el método de compresión PPMd dentro de un archivo 7z.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | Instancia la configuración para el método de compresión PPMd dentro del archivo 7z. |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | Instancia la configuración para el método de compresión PPMd dentro del archivo 7z con el orden de modelo predeterminado y el tamaño del subasignador. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | Obtiene el orden máximo. |
| [getMethod()](#getMethod--) | Obtiene el método de compresión o descompresión. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Obtiene el tamaño del subasignador en MB. |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


Instancia la configuración para el método de compresión PPMd dentro del archivo 7z.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32)))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| maxOrder | int | Maximum order.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### SevenZipPPMdCompressionSettings() {#SevenZipPPMdCompressionSettings--}
```
public SevenZipPPMdCompressionSettings()
```


Instantiates settings for PPMd compression method within 7z archive with default model order and sub-allocator size.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("sevenZipFile.7z");
     }
 
```

El orden de modelo predeterminado es 6 y el tamaño del subasignador es 16 MB.

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


Obtiene el orden máximo.

**Returns:**
byte - el orden máximo
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Obtiene el método de compresión o descompresión.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Obtiene el tamaño del subasignador en MB.

**Returns:**
int - el tamaño del subasignador en MB
