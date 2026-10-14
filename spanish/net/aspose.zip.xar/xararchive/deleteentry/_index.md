---
title: "XarArchive.DeleteEntry"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método XarArchive. Elimina la primera aparición de una entrada específica de la lista de entradas"
type: docs
weight: 50
url: /es/net/aspose.zip.xar/xararchive/deleteentry/
---
## XarArchive.DeleteEntry method

Elimina la primera aparición de una entrada específica de la lista de entradas.

```csharp
public XarArchive DeleteEntry(XarEntry entry)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| entrada | XarEntry | La entrada a eliminar de la lista de entradas. |

### Valor devuelto

Instancia de entrada Xar.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *entry* es nulo. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| InvalidOperationException | El archivo no está abierto para extracción. |

## Ejemplos

Así es como puedes eliminar todas las entradas excepto la última:

```csharp
using (var archive = new XarArchive("archive.xar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries.FirstOrDefault());
    archive.Save(outputXarFile);
}
```

### Ver también

* class [XarEntry](../../xarentry/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


