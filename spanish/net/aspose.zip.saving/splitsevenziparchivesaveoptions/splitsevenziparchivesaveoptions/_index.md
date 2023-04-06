---
title: SplitSevenZipArchiveSaveOptions.SplitSevenZipArchiveSaveOptions
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SplitSevenZipArchiveSaveOptions constructor. Instancia la configuración para guardar un archivo 7z de varios volúmenes.
type: docs
weight: 10
url: /es/net/aspose.zip.saving/splitsevenziparchivesaveoptions/splitsevenziparchivesaveoptions/
---
## SplitSevenZipArchiveSaveOptions constructor

Instancia la configuración para guardar un archivo 7z de varios volúmenes.

```csharp
public SplitSevenZipArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fileName | String | Nombre de los volúmenes. Puede ser con o sin extensión .7z. |
| segmentSize | UInt32 | Tamaño del volumen. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentOutOfRangeException | *segmentSize* es menos de 100. |

### Observaciones

Algunos volúmenes pueden ser inferiores a*segmentSize*. En la mayoría de los casos, el último segmento será menor, pero rara vez los segmentos regulares también lo serán.

Los nombres de los archivos serán los siguientes:*fileName* .7z.001,*fileName* .7z.002, ...,*fileName*.7z.(n).

### Ver también

* class [SplitSevenZipArchiveSaveOptions](../)
* espacio de nombres [Aspose.Zip.Saving](../../splitsevenziparchivesaveoptions/)
* asamblea [Aspose.Zip](../../../)


