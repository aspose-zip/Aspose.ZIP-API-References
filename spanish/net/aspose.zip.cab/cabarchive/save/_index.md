---
title: "CabArchive.Save"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método CabArchive. Guarda el archivo en el flujo proporcionado"
type: docs
weight: 70
url: /es/net/aspose.zip.cab/cabarchive/save/
---
## Save(Stream, CabSaveOptions) {#save}

Guarda el archivo en el flujo proporcionado.

```csharp
public void Save(Stream outputStream, CabSaveOptions saveOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| outputStream | Flujo | Flujo de destino. |
| saveOptions | CabSaveOptions | Opciones para guardar el archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | *outputStream* no es escribible ni buscable. |
| ObjectDisposedException | El archivo ha sido descartado. |
| InvalidOperationException | El archivo está preparado para extracción y no puede guardarse. |

## Observaciones

*outputStream* must be writable.

## Ejemplos

```csharp
using (FileStream cabFile = File.Open("archive.cab", FileMode.Create))
{
    using (var archive = new CabArchive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(cabFile);
    }
}
```

### Ver también

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, CabSaveOptions) {#save_1}

Guarda el archivo en el archivo de destino proporcionado.

```csharp
public void Save(string destinationFileName, CabSaveOptions saveOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationFileName | String | La ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito. |
| saveOptions | CabSaveOptions | Opciones para guardar el archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *destinationFileName* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder. |
| ArgumentException | El *destinationFileName* está vacío, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *destinationFileName* denegado. |
| PathTooLongException | El *destinationFileName* especificado, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *destinationFileName* contiene dos puntos (:) en medio de la cadena. |
| FileNotFoundException | El archivo no se encuentra. |
| InvalidOperationException | El archivo está abierto para extracción. |
| DirectoryNotFoundException | La ruta especificada no es válida, como por ejemplo estar en una unidad no asignada. |
| IOException | El archivo ya está abierto. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Observaciones

Es posible guardar un archivo en la misma ruta desde la que se cargó. Sin embargo, no se recomienda porque este enfoque usa la copia a un archivo temporal.

## Ejemplos

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### Ver también

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


