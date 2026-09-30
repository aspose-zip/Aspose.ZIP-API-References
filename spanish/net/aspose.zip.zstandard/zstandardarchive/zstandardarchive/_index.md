---
title: "ZstandardArchive.ZstandardArchive"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Constructor de ZstandardArchive. Inicializa una nueva instancia de la clase ZstandardArchive preparada para comprimir"
type: docs
weight: 10
url: /es/net/aspose.zip.zstandard/zstandardarchive/zstandardarchive/
---
## ZstandardArchive() {#constructor}

Inicializa una nueva instancia de la clase [`ZstandardArchive`](../) preparada para comprimir.

```csharp
public ZstandardArchive()
```

## Ejemplos

El siguiente ejemplo muestra cómo comprimir un archivo.

```csharp
using (ZstandardArchive archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### Ver también

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(Stream, ZstandardLoadOptions) {#constructor_1}

Inicializa una nueva instancia de la clase [`ZstandardArchive`](../) preparada para descomprimir.

```csharp
public ZstandardArchive(Stream sourceStream, ZstandardLoadOptions options = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | Flujo | La fuente del archivo. |
| opciones | ZstandardLoadOptions | Las opciones con las que cargar el archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | Se lanza si el flujo de origen ha sido eliminado. |
| EndOfStreamException | Se lanza cuando se alcanza inesperadamente el final del flujo. |
| IOException | Se produce un error de E/S. |
| InvalidDataException | Se lanza cuando los datos son inválidos o están corruptos. |

## Observaciones

Este constructor no descomprime. Consulte el método [`Open`](../open/) para descomprimir.

## Ejemplos

Abra un archivo desde un flujo y extráigalo a un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new ZstandardArchive(File.OpenRead("archive.zst")))
  archive.Open().CopyTo(ms);
```

### Ver también

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(string, ZstandardLoadOptions) {#constructor_2}

Inicializa una nueva instancia de la clase [`ZstandardArchive`](../).

```csharp
public ZstandardArchive(string path, ZstandardLoadOptions options = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta al archivo de archivo. |
| opciones | ZstandardLoadOptions | Las opciones con las que cargar el archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder. |
| ArgumentException | La *path* está vacía, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *path* denegado. |
| PathTooLongException | La *path* especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *path* contiene dos puntos (:) en medio de la cadena. |
| DirectoryNotFoundException | La ruta especificada no es válida, como por ejemplo estar en una unidad no asignada. |
| EndOfStreamException | Se lanza cuando se alcanza inesperadamente el final del flujo. |
| FileNotFoundException | El archivo no se encuentra. |
| IOException | El archivo ya está abierto. |
| InvalidDataException | Se lanza cuando los datos son inválidos o están corruptos. |

## Observaciones

Este constructor no descomprime. Consulte el método [`Open`](../open/) para descomprimir.

## Ejemplos

Abra un archivo desde la ruta del archivo y extráigalo a un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (ZstandardArchive archive = new ZstandardArchive("archive.zst"))
  archive.Open().CopyTo(ms);
```

### Ver también

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


