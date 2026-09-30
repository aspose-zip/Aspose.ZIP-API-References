---
title: "TarArchive.FromZstandard"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método TarArchive. Extrae el archivo Zstandard suministrado y compone TarArchive a partir de los datos extraídos"
type: docs
weight: 80
url: /es/net/aspose.zip.tar/tararchive/fromzstandard/
---
## FromZstandard(Stream) {#fromzstandard}

Extrae el archivo Zstandard suministrado y compone [`TarArchive`](../) a partir de los datos extraídos.

Importante: el archivo Zstandard se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga cuidado con el consumo de memoria.

```csharp
public static TarArchive FromZstandard(Stream source)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | Flujo | La fuente del archivo. |

### Valor devuelto

Una instancia de [`TarArchive`](../)

### Excepciones

| excepción | condición |
| --- | --- |
| IOException | El flujo Zstandard está corrupto o no es legible. |
| InvalidDataException | Los datos están corruptos. |
| EndOfStreamException | Se lanza cuando se alcanza el final del flujo antes de que se lean la cantidad esperada de bytes. |
| ObjectDisposedException | Se lanza si el flujo de origen ha sido eliminado. |

### Ver también

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromZstandard(string) {#fromzstandard_1}

Extrae el archivo Zstandard suministrado y compone [`TarArchive`](../) a partir de los datos extraídos.

Importante: el archivo Zstandard se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga cuidado con el consumo de memoria.

```csharp
public static TarArchive FromZstandard(string path)
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
| IOException | El flujo Zstandard está corrupto o no es legible. |
| InvalidDataException | Los datos están corruptos. |
| EndOfStreamException | Se lanza cuando se alcanza el final del flujo antes de que se lean la cantidad esperada de bytes. |

### Ver también

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


