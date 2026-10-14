---
title: "LzipArchiveSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "La clase contiene la configuración de un archivo lzip particular."
type: docs
weight: 84
url: /es/java/com.aspose.zip/lziparchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzipArchiveSettings
```

La clase contiene la configuración de un archivo lzip particular.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LzipArchiveSettings(int dictionarySize)](#LzipArchiveSettings-int-) | Inicializa una nueva instancia de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con un tamaño de diccionario particular. |
| [LzipArchiveSettings(int dictionarySize, int maxMemberSize)](#LzipArchiveSettings-int-int-) | Inicializa una nueva instancia de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con un tamaño de diccionario particular. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Obtiene el recuento de hilos de compresión. |
| [getDictionarySize()](#getDictionarySize--) | Obtiene el tamaño del diccionario que se usa en la compresión LZMA. |
| [getFastSpeed()](#getFastSpeed--) | Obtiene la instancia de la clase [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con un tamaño de diccionario igual a 1 megabyte en el filtro LZMA. |
| [getFastestSpeed()](#getFastestSpeed--) | Obtiene la instancia de la clase [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con un tamaño de diccionario igual a 65536 bytes en el filtro LZMA. |
| [getHighCompression()](#getHighCompression--) | Obtiene la instancia de la clase [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con un tamaño de diccionario igual a 32 megabytes en el filtro LZMA. |
| [getMaxMemberSize()](#getMaxMemberSize--) | Obtiene el tamaño máximo de un miembro en un archivo lzip presentado en bytes. |
| [getMaximumCompression()](#getMaximumCompression--) | Obtiene la instancia de la clase [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con un tamaño de diccionario igual a 64 megabytes en el filtro LZMA. |
| [getNormal()](#getNormal--) | Obtiene la instancia de la clase [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con un tamaño de diccionario igual a 16 megabytes en el filtro LZMA. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Establece el recuento de hilos de compresión. |
### LzipArchiveSettings(int dictionarySize) {#LzipArchiveSettings-int-}
```
public LzipArchiveSettings(int dictionarySize)
```


Inicializa una nueva instancia de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con un tamaño de diccionario particular.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dictionarySize | int | tamaño del diccionario para la compresión LZMA en bytes |

### LzipArchiveSettings(int dictionarySize, int maxMemberSize) {#LzipArchiveSettings-int-int-}
```
public LzipArchiveSettings(int dictionarySize, int maxMemberSize)
```


Inicializa una nueva instancia de [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con un tamaño de diccionario particular.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dictionarySize | int | tamaño del diccionario para la compresión LZMA en bytes |
| maxMemberSize | int | Tamaño máximo de un miembro en un archivo lzip presentado en bytes. El valor predeterminado es 60 MB. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Obtiene el recuento de hilos de compresión. Si el valor es mayor que 1, se utilizará compresión multihilo.

**Returns:**
int - recuento de hilos de compresión
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Obtiene el tamaño del diccionario que se usa en la compresión LZMA.

**Returns:**
int - el tamaño del diccionario que se usa en la compresión LZMA
### getFastSpeed() {#getFastSpeed--}
```
public static LzipArchiveSettings getFastSpeed()
```


Obtiene la instancia de la clase [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con un tamaño de diccionario igual a 1 megabyte en el filtro LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 1 megabyte in LZMA filter
### getFastestSpeed() {#getFastestSpeed--}
```
public static LzipArchiveSettings getFastestSpeed()
```


Obtiene la instancia de la clase [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con un tamaño de diccionario igual a 65536 bytes en el filtro LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 65536 bytes in LZMA filter
### getHighCompression() {#getHighCompression--}
```
public static LzipArchiveSettings getHighCompression()
```


Obtiene la instancia de la clase [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con un tamaño de diccionario igual a 32 megabytes en el filtro LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 32 megabytes in LZMA filter
### getMaxMemberSize() {#getMaxMemberSize--}
```
public final long getMaxMemberSize()
```


Obtiene el tamaño máximo de un miembro en un archivo lzip presentado en bytes.

**Returns:**
long - el tamaño máximo de un miembro en un archivo lzip presentado en bytes
### getMaximumCompression() {#getMaximumCompression--}
```
public static LzipArchiveSettings getMaximumCompression()
```


Obtiene la instancia de la clase [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con un tamaño de diccionario igual a 64 megabytes en el filtro LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 64 megabytes in LZMA filter
### getNormal() {#getNormal--}
```
public static LzipArchiveSettings getNormal()
```


Obtiene la instancia de la clase [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) con un tamaño de diccionario igual a 16 megabytes en el filtro LZMA.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the instance of the [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) class with dictionary size equals to 16 megabytes in LZMA filter
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Establece el recuento de hilos de compresión. Si el valor es mayor que 1, se utilizará compresión multihilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | recuento de hilos de compresión |

