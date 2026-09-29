---
title: "SplitSevenZipArchiveSaveOptions"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Opciones para guardar un archivo 7-zip de varios volúmenes."
type: docs
weight: 123
url: /es/java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

Opciones para guardar un archivo 7-zip de varios volúmenes.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | Instancia la configuración para guardar un archivo 7z de varios volúmenes. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getFileName()](#getFileName--) | Obtiene el nombre de los segmentos sin extensión. |
| [getSegmentSize()](#getSegmentSize--) | Obtiene el tamaño del segmento. |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


Instancia la configuración para guardar un archivo 7z de varios volúmenes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | fileName | java.lang.String | nombre para los volúmenes. Puede ser con o sin la extensión .7z. |

Los nombres de los archivos serán los siguientes: `fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
|  | segmentSize | long | tamaño del volumen. |

Algunos volúmenes pueden ser menores que `segmentSize`. En la mayoría de los casos, el último segmento será menor, pero rara vez los segmentos regulares podrían ser también. |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Obtiene el nombre de los segmentos sin extensión.

**Returns:**
java.lang.String - el nombre de los segmentos sin extensión
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Obtiene el tamaño del segmento.

**Returns:**
long - el tamaño del segmento.
