---
title: "IsoArchive.CreateDirectory"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método IsoArchive. Añade un directorio a la imagen ISO"
type: docs
weight: 30
url: /es/net/aspose.zip.iso/isoarchive/createdirectory/
---
## IsoArchive.CreateDirectory method

Agrega un directorio a la imagen ISO.

```csharp
public IsoEntry CreateDirectory(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | Ruta del directorio en el ISO. |

### Valor devuelto

La entrada ISO compuesta.

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | El archivo está abierto para extracción. |
| ArgumentNullException | `name` es null o está vacío. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

### Ver también

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


