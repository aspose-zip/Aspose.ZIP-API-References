---
title: "ArjArchive.ExtractToDirectory"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método ArjArchive. Extrae todas las entradas al directorio especificado."
type: docs
weight: 60
url: /es/net/aspose.zip.arj/arjarchive/extracttodirectory/
---
## ArjArchive.ExtractToDirectory method

Extrae todas las entradas al directorio especificado.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationDirectory | String | El directorio donde extraer las entradas. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | Se lanza cuando el *destinationDirectory* es nulo. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |
| InvalidDataException | Desajuste de suma de verificación para encabezados o datos. - o - El archivo está corrupto. |
| NotImplementedException | Entrada comprimida con el método 4. |

## Ejemplos

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio:

```csharp
using (var archive = new ArjArchive(File.OpenRead("archive.arj")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Ver también

* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


