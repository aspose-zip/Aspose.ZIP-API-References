---
title: "LzxArchive.LzxArchive"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Constructor LzxArchive. Inicializa una nueva instancia de la clase LzxArchive y compone una lista de entradas que puede ser extraída del archivo"
type: docs
weight: 10
url: /es/net/aspose.zip.lzx/lzxarchive/lzxarchive/
---
## LzxArchive(Stream, LzxLoadOptions) {#constructor}

Inicializa una nueva instancia de la clase [`LzxArchive`](../) y compone una lista de entradas que puede ser extraída del archivo.

```csharp
public LzxArchive(Stream extractionSource, LzxLoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| extractionSource | Flujo | La fuente del archivo. |
| loadOptions | LzxLoadOptions | Opciones para cargar el archivo existente. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *extractionSource* es nulo. |
| ArgumentException | *extractionSource* no admite búsqueda. |
| InvalidDataException | Firma incorrecta para el archivo. - o - El archivo no es un archivo LZX. |
| NotImplementedException | El archivo Lzx contiene entradas combinadas. |
| EndOfStreamException | El flujo *extractionSource* es demasiado corto. |
| ObjectDisposedException | Se lanza si el flujo ha sido cerrado. |
| IOException | Se produce un error de E/S. |

## Observaciones

Este constructor no descomprime ninguna entrada. Consulte el método [`Extract`](../../lzxarchiveentry/extract/) para descomprimir.

### Ver también

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzxArchive(string, LzxLoadOptions) {#constructor_1}

Inicializa una nueva instancia de la clase [`LzxArchive`](../) y compone una lista de entradas que puede ser extraída del archivo.

```csharp
public LzxArchive(string path, LzxLoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta completa o relativa al archivo del archivo. |
| loadOptions | LzxLoadOptions | Opciones para cargar el archivo existente. |

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
| InvalidDataException | El archivo está corrupto. |
| NotImplementedException | El archivo Lzx contiene entradas combinadas. |
| EndOfStreamException | El archivo es demasiado corto. |
| ObjectDisposedException | Se lanza si el flujo ha sido cerrado. |

## Observaciones

Este constructor no descomprime ninguna entrada. Consulte el método [`Extract`](../../lzxarchiveentry/extract/) para descomprimir.

## Ejemplos

El siguiente ejemplo extrae un archivo, luego descomprime la primera entrada a un `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LzxArchive archive = new LzxArchive("sample.lzx"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Ver también

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


