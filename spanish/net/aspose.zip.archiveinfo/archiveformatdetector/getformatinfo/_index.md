---
title: "GetFormatInfo"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: 
type: docs
weight: 20
url: /es/net/aspose.zip.archiveinfo/archiveformatdetector/getformatinfo/
---
## ArchiveFormatDetector.GetFormatInfo method (1 of 2)

Obtiene información de formato.

```csharp
public ArchiveFormatInfo GetFormatInfo(string fileName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | String | El nombre de archivo del archivo de archivo. |

### Valor devuelto

Información sobre el formato del archivo o null si no se detectó el formato.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *fileName* es null. |
| SecurityException | El llamador no tiene el permiso requerido para acceder. |
| ArgumentException | El *fileName* está vacío, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | El acceso al archivo *fileName* está denegado. |
| PathTooLongException | El *fileName* especificado supera la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo deben tener menos de 260 caracteres. |
| NotSupportedException | El archivo en *fileName* contiene dos puntos (:) en medio de la cadena. |
| IOException | Se produjo un error de E/S al abrir el archivo. |

### Ver también

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

---

## ArchiveFormatDetector.GetFormatInfo method (2 of 2)

Obtiene información de formato.

```csharp
public ArchiveFormatInfo GetFormatInfo(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | El flujo del archivo de archivo. |

### Valor devuelto

Información sobre el formato del archivo o null si no se detectó el formato.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *stream* es nulo. |
| ArgumentException | *stream* no es buscable. |

### Ver también

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

<!-- NO EDITAR: generado por xmldocmd para Aspose.Zip.dll -->
