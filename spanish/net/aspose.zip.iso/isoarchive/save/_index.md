---
title: "IsoArchive.Save"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método IsoArchive. Guarda la imagen ISO en la ruta especificada."
type: docs
weight: 70
url: /es/net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

Guarda la imagen ISO en la ruta especificada.

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta donde se guardará la imagen ISO. |
| saveOptions | IsoSaveOptions | Opciones para guardar el archivo ISO. |

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Se lanza cuando el archivo no está en modo de edición. |
| ArgumentNullException | Se lanza cuando *path* es nulo. |
| DirectoryNotFoundException | Se lanza cuando la ruta especificada no es válida, como por estar en una unidad no asignada. |
| IOException | Se lanza cuando el archivo ya está abierto. |
| UnauthorizedAccessException | Se lanza cuando se niega el acceso al archivo *path*. |
| PathTooLongException | Se lanza cuando la *path* especificada supera la longitud máxima definida por el sistema. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Ejemplos

El siguiente ejemplo muestra cómo guardar un archivo ISO en un archivo:

```csharp
// Crear un nuevo archivo ISO vacío
using(IsoArchive isoArchive = new IsoArchive())
{
    // Agregar archivos al archivo ISO
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Guardar el archivo ISO en un archivo
    isoArchive.Save("new_archive.iso");
}
```

### Ver también

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

Guarda la imagen ISO en el flujo especificado.

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | Flujo | La secuencia donde se guardará la imagen ISO. |
| saveOptions | IsoSaveOptions | Opciones para guardar el archivo ISO. |

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Se lanza cuando el archivo no está en modo de edición. |
| ArgumentNullException | Se lanza cuando *stream* es nulo. |
| ArgumentException | Se lanza cuando el *stream* no es escribible. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| IOException | Se produce un error de E/S. |

## Ejemplos

El siguiente ejemplo muestra cómo guardar un archivo ISO en un flujo de memoria:

```csharp

 // Crear un nuevo archivo ISO vacío
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // Agregar archivos al archivo ISO
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // Guardar el archivo ISO en un flujo de memoria
     isoArchive.Save(memoryStream);
 }
```

### Ver también

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


