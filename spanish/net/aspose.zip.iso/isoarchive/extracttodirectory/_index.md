---
title: "IsoArchive.ExtractToDirectory"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método IsoArchive. Extrae todas las entradas al directorio especificado"
type: docs
weight: 60
url: /es/net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

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
| InvalidOperationException | Se lanza cuando el archivo está en modo de edición. |
| ArgumentNullException | Se lanza cuando el *destinationDirectory* es nulo. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Ejemplos

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio:

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Ver también

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


