---
title: "ArchiveFormatDetector"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Detecta un formato de archivo y proporciona otra información relacionada."
type: docs
weight: 32
url: /es/java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

Detecta un formato de archivo y proporciona otra información relacionada.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | Inicializa una nueva instancia de la clase [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | Obtiene información del formato. |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | Obtiene información del formato. |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


Inicializa una nueva instancia de la clase [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector).

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


Obtiene información del formato.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | El flujo del archivo del archivo. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


Obtiene información del formato.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre de archivo del archivo del archivo. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
