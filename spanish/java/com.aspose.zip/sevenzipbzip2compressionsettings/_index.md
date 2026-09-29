---
title: "SevenZipBZip2CompressionSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración para el método de compresión BZip2 dentro de un archivo 7z."
type: docs
weight: 109
url: /es/java/com.aspose.zip/sevenzipbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipBZip2CompressionSettings extends SevenZipCompressionSettings
```

Configuración para el método de compresión BZip2 dentro de un archivo 7z.

Bzip2 comprime archivos usando el algoritmo de compresión de texto por ordenación de bloques Burrows-Wheeler y la codificación Huffman.

Ver más: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SevenZipBZip2CompressionSettings(int blockSize)](#SevenZipBZip2CompressionSettings-int-) | Inicializa una nueva instancia de la clase [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings). |
| [SevenZipBZip2CompressionSettings()](#SevenZipBZip2CompressionSettings--) | Inicializa una nueva instancia de la clase [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) con el tamaño de bloque predeterminado, igual a 9 cientos de kilobytes. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Tamaño de bloque en cientos de kilobytes. |
| [getMethod()](#getMethod--) | Obtiene el método de compresión o descompresión. |
### SevenZipBZip2CompressionSettings(int blockSize) {#SevenZipBZip2CompressionSettings-int-}
```
public SevenZipBZip2CompressionSettings(int blockSize)
```


Inicializa una nueva instancia de la clase [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| blockSize | int | tamaño de bloque en cientos de kilobytes |

### SevenZipBZip2CompressionSettings() {#SevenZipBZip2CompressionSettings--}
```
public SevenZipBZip2CompressionSettings()
```


Inicializa una nueva instancia de la clase [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) con el tamaño de bloque predeterminado, igual a 9 cientos de kilobytes.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Tamaño de bloque en cientos de kilobytes.

**Returns:**
int - tamaño de bloque en cientos de kilobytes
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Obtiene el método de compresión o descompresión.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
