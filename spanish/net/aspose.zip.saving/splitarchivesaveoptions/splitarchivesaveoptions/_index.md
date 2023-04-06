---
title: SplitArchiveSaveOptions.SplitArchiveSaveOptions
second_title: Referencia de la API de Aspose.ZIP para .NET
description: SplitArchiveSaveOptions constructor. Instancia la configuración para guardar un archivo zip de varios volúmenes.
type: docs
weight: 10
url: /es/net/aspose.zip.saving/splitarchivesaveoptions/splitarchivesaveoptions/
---
## SplitArchiveSaveOptions constructor

Instancia la configuración para guardar un archivo zip de varios volúmenes.

```csharp
public SplitArchiveSaveOptions(string fileName, uint segmentSize)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fileName | String | Nombre de los volúmenes. Puede ser con o sin extensión .zip. |
| segmentSize | UInt32 | Tamaño del volumen. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentOutOfRangeException | El tamaño del segmento es inferior a 65536 bytes. |

### Observaciones

Algunos volúmenes pueden ser inferiores a*segmentSize*. En la mayoría de los casos, el último segmento será menor, pero rara vez los segmentos regulares también lo serán.

Los nombres de los archivos serán los siguientes:*fileName* .z01,*fileName* .z02, ...,*fileName* .z(n-1),*fileName*.cremallera.

### Ver también

* class [SplitArchiveSaveOptions](../)
* espacio de nombres [Aspose.Zip.Saving](../../splitarchivesaveoptions/)
* asamblea [Aspose.Zip](../../../)


