---
title: "XarArchive.Save"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método XarArchive. Guarda el archivo en el archivo de destino proporcionado"
type: docs
weight: 80
url: /es/net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

Guarda el archivo en el archivo de destino proporcionado.

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationFileName | String | La ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito. |
| saveOptions | XarSaveOptions | Opciones para guardar el archivo xar. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *destinationFileName* es nulo. |
| InvalidOperationException | Imposible modificar el archivo xar. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| IOException | Se produjo un error de E/S al abrir el archivo. |
| PathTooLongException | La ruta especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. |
| UnauthorizedAccessException | *destinationFileName* especificó un archivo de solo lectura. -or- *destinationFileName* especificó un directorio. -or- El llamador no tiene el permiso requerido. |

### Ver también

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

Guarda el archivo en el flujo proporcionado.

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| salida | Flujo | Flujo de destino. |
| saveOptions | XarSaveOptions | Opciones para guardar el archivo xar. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *output* es nulo. |
| ArgumentException | *output* no es escribible/legible o no es buscable. |
| InvalidOperationException | Imposible modificar el archivo xar. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

### Ver también

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


