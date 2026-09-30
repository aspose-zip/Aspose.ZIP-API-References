---
title: "ArjArchive.ArjArchive"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Constructor de ArjArchive. Inicializa una nueva instancia de la clase ArjArchive y compone una lista de entradas que pueden extraerse del archivo."
type: docs
weight: 10
url: /es/net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream, ArjLoadOptions) {#constructor}

Inicializa una nueva instancia de la clase [`ArjArchive`](../) y compone una lista de entradas que pueden extraerse del archivo.

```csharp
public ArjArchive(Stream extractionSource, ArjLoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| extractionSource | Flujo | La fuente del archivo. |
| loadOptions | ArjLoadOptions | Opciones para cargar el archivo existente. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *extractionSource* es nulo. |
| ArgumentException | &gt;*extractionSource* no admite búsqueda. |
| InvalidDataException | Firma incorrecta para el archivo. - o - El archivo no es un archivo ARJ. |
| EndOfStreamException | Lanzado cuando se alcanza el final del flujo antes de que se hayan leído todos los bytes de encabezado o de nombre. |
| NotSupportedException | El archivo está dañado. |

## Observaciones

Este constructor no descomprime ninguna entrada. Consulte el método [`Extract`](../../arjentryplain/extract/) para descomprimir.

### Ver también

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string, ArjLoadOptions) {#constructor_1}

Inicializa una nueva instancia de la clase [`ArjArchive`](../) y compone una lista de entradas que pueden extraerse del archivo.

```csharp
public ArjArchive(string path, ArjLoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta al archivo de archivo. |
| loadOptions | ArjLoadOptions | Opciones para cargar el archivo existente. |

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
| EndOfStreamException | Lanzado cuando se alcanza el final del flujo antes de que se hayan leído todos los bytes de encabezado o de nombre. |
| InvalidDataException | El número mágico de ARJ es inválido o el tamaño del encabezado está fuera de rango. |

## Observaciones

Este constructor no desempaqueta ninguna entrada. Consulte el método [`Extract`](../../arjentryplain/extract/) para descomprimir.

## Ejemplos

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Ver también

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


