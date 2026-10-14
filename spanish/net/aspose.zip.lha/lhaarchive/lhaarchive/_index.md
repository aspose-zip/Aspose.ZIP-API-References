---
title: "LhaArchive.LhaArchive"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Constructor LhaArchive. Inicializa una nueva instancia de la clase LhaArchive y compone una lista de entradas que pueden extraerse del archivo."
type: docs
weight: 10
url: /es/net/aspose.zip.lha/lhaarchive/lhaarchive/
---
## LhaArchive(Stream, LhaLoadOptions) {#constructor}

Inicializa una nueva instancia de la clase [`LhaArchive`](../) y compone una lista de entradas que pueden extraerse del archivo.

```csharp
public LhaArchive(Stream sourceStream, LhaLoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | Flujo | La fuente del archivo. |
| loadOptions | LhaLoadOptions | Opciones para cargar el archivo existente. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *sourceStream* es nulo |
| ArgumentException | *sourceStream* no es buscable. |
| InvalidDataException | Se encontraron datos inapropiados. |
| EndOfStreamException | Se lanza cuando se alcanza el final del flujo antes de que se lean la cantidad esperada de bytes. |
| ObjectDisposedException | Lanzado cuando el objeto ha sido eliminado. |

## Observaciones

Este constructor no descomprime ninguna entrada. Consulte el método [`Extract`](../../lhaarchiveentry/extract/) para descomprimir.

### Ver también

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LhaArchive(string, LhaLoadOptions) {#constructor_1}

Inicializa una nueva instancia de la clase [`LhaArchive`](../) y compone una lista de entradas que pueden extraerse del archivo.

```csharp
public LhaArchive(string path, LhaLoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta completa o relativa al archivo del archivo. |
| loadOptions | LhaLoadOptions | Opciones para cargar el archivo existente. |

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
| EndOfStreamException | Se lanza cuando se alcanza el final del flujo antes de que se lean la cantidad esperada de bytes. |
| ObjectDisposedException | Lanzado cuando el objeto ha sido eliminado. |

## Observaciones

Este constructor no descomprime ninguna entrada. Consulte el método [`Extract`](../../lhaarchiveentry/extract/) para descomprimir.

## Ejemplos

El siguiente ejemplo extrae un archivo, luego descomprime la primera entrada a un `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LhaArchive archive = new LhaArchive("sample.lzh"))
{
    archive.Entries[0].Extract(extracted);
}
```

### Ver también

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


