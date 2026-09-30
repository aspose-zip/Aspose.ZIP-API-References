---
title: "TarArchive.FromLZ4"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método TarArchive. Extrae el archivo LZ4 suministrado y compone TarArchive a partir de los datos extraídos"
type: docs
weight: 30
url: /es/net/aspose.zip.tar/tararchive/fromlz4/
---
## FromLZ4(string) {#fromlz4_1}

Extrae el archivo LZ4 suministrado y compone [`TarArchive`](../) a partir de los datos extraídos.

Importante: el archivo LZ4 se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga cuidado con el consumo de memoria.

```csharp
public static TarArchive FromLZ4(string path)
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
| SecurityException | El llamador no tiene el permiso requerido para acceder |
| ArgumentException | La *path* está vacía, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *path* denegado. |
| PathTooLongException | La *path* especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *path* tiene un formato no válido. |
| DirectoryNotFoundException | La ruta especificada no es válida, como por ejemplo estar en una unidad no asignada. |
| FileNotFoundException | El archivo no se encuentra. |
| EndOfStreamException | El archivo es demasiado corto. |
| InvalidDataException | El archivo tiene una firma incorrecta. |
| IOException | Se produjo un error de E/S al abrir el archivo. |
| InvalidOperationException | El archivo está preparado para la composición. |

## Observaciones

El flujo de extracción LZ4 no es desplazable debido a la naturaleza del algoritmo de compresión. El archivo Tar proporciona una funcionalidad para extraer registros arbitrarios, por lo que debe operar con un flujo desplazable internamente.

### Ver también

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZ4(Stream) {#fromlz4}

Extrae el archivo LZ4 suministrado y compone [`TarArchive`](../) a partir de los datos extraídos.

Importante: el archivo LZ4 se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga cuidado con el consumo de memoria.

```csharp
public static TarArchive FromLZ4(Stream source)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | Flujo | La fuente del archivo. |

### Valor devuelto

Una instancia de [`TarArchive`](../)

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | No se puede leer de *source* |
| ArgumentNullException | *source* es nulo. |
| EndOfStreamException | *source* es demasiado corto. |
| InvalidDataException | El *source* tiene una firma incorrecta. |
| ObjectDisposedException | Se lanza si el flujo de origen ha sido eliminado. |

## Observaciones

El flujo de extracción LZ4 no es desplazable debido a la naturaleza del algoritmo de compresión. El archivo Tar proporciona una funcionalidad para extraer registros arbitrarios, por lo que debe operar con un flujo desplazable internamente.

### Ver también

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


