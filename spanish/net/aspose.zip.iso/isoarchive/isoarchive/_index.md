---
title: "IsoArchive.IsoArchive"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Constructor de IsoArchive. Inicializa una nueva instancia de la clase IsoArchive y crea un archivo ISO vacío para agregar nuevos archivos y directorios"
type: docs
weight: 10
url: /es/net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

Inicializa una nueva instancia de la clase [`IsoArchive`](../) y crea un archivo ISO vacío para agregar nuevos archivos y directorios.

```csharp
public IsoArchive()
```

## Ejemplos

El siguiente ejemplo muestra cómo crear un nuevo archivo ISO vacío y agregar archivos a él:

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

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

Inicializa una nueva instancia de la clase [`IsoArchive`](../) y compone una lista de entradas que se puede extraer del archivo.

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | Flujo | El origen del archivo. Debe ser desplazable. |
| loadOptions | IsoLoadOptions | Las opciones con las que cargar el archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *sourceStream* es nulo. |
| ArgumentException | *sourceStream* no es desplazable. |
| InvalidDataException | *sourceStream* no es un archivo ISO válido. |
| ObjectDisposedException | Se lanza si el flujo de origen ha sido eliminado. |
| EndOfStreamException | Se lanza cuando se alcanza inesperadamente el final del flujo. |
| IOException | Se produce un error de E/S. |
| NotSupportedException | El flujo no admite lectura. |

## Observaciones

Este constructor no desempaqueta ninguna entrada.

## Ejemplos

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Ver también

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

Inicializa una nueva instancia de la clase [`IsoArchive`](../) y compone una lista de entradas que se puede extraer del archivo.

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta al archivo de archivo. |
| loadOptions | IsoLoadOptions | Las opciones con las que cargar el archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder. |
| ArgumentException | La *path* está vacía, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *path* denegado. |
| PathTooLongException | La *path* especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *path* contiene dos puntos (:) en medio de la cadena. |
| FileNotFoundException | El archivo no se encuentra. |
| DirectoryNotFoundException | La ruta especificada no es válida, como por ejemplo estar en una unidad no asignada. |
| IOException | El archivo ya está abierto. |
| EndOfStreamException | El archivo es demasiado corto. |
| InvalidDataException | Se lanza cuando los datos son inválidos o están corruptos. |

## Observaciones

Este constructor no desempaqueta ninguna entrada.

## Ejemplos

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Ver también

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


