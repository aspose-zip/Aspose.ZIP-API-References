---
title: "TarArchive.FromLZMA"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método TarArchive. Extrae el archivo LZMA suministrado y compone TarArchive a partir de los datos extraídos"
type: docs
weight: 50
url: /es/net/aspose.zip.tar/tararchive/fromlzma/
---
## FromLZMA(Stream) {#fromlzma}

Extrae el archivo LZMA suministrado y compone [`TarArchive`](../) a partir de los datos extraídos.

Importante: el archivo LZMA se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga cuidado con el consumo de memoria.

```csharp
public static TarArchive FromLZMA(Stream source)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | Flujo | La fuente del archivo. |

### Valor devuelto

Una instancia de [`TarArchive`](../)

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidDataException | El archivo está corrupto. |
| EndOfStreamException | Se lanza cuando se alcanza el final del flujo antes de que se lean la cantidad esperada de bytes. |
| ObjectDisposedException | Se lanza si el flujo de origen ha sido eliminado. |
| ArgumentNullException | *source* es nulo. |
| IOException | Se produce un error de E/S. |

## Observaciones

El flujo de extracción LZMA no es buscable por la naturaleza del algoritmo de compresión. El archivo Tar proporciona la capacidad de extraer registros arbitrarios, por lo que debe operar con un flujo buscable internamente.

### Ver también

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZMA(string) {#fromlzma_1}

Extrae el archivo LZMA suministrado y compone [`TarArchive`](../) a partir de los datos extraídos.

Importante: el archivo LZMA se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga cuidado con el consumo de memoria.

```csharp
public static TarArchive FromLZMA(string path)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta al archivo de archivo. |

### Valor devuelto

Una instancia de [`TarArchive`](../)

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| ArgumentException | La *path* está vacía, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *path* denegado. |
| PathTooLongException | La *path* especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *path* tiene un formato no válido. |
| DirectoryNotFoundException | La ruta especificada no es válida, como por ejemplo estar en una unidad no asignada. |
| FileNotFoundException | El archivo no se encuentra. |
| EndOfStreamException | Se lanza cuando se alcanza el final del flujo antes de que se lean la cantidad esperada de bytes. |
| IOException | Se produjo un error de E/S al abrir el archivo. |
| InvalidDataException | El archivo está corrupto. |

## Observaciones

El flujo de extracción LZMA no es buscable por la naturaleza del algoritmo de compresión. El archivo Tar proporciona la capacidad de extraer registros arbitrarios, por lo que debe operar con un flujo buscable internamente.

### Ver también

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


