---
title: "Lz4Archive.Lz4Archive"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Constructor Lz4Archive. Inicializa una nueva instancia de la clase Lz4Archive preparada para descomprimir"
type: docs
weight: 10
url: /es/net/aspose.zip.lz4/lz4archive/lz4archive/
---
## Lz4Archive(Stream, Lz4LoadOptions) {#constructor_1}

Inicializa una nueva instancia de la clase [`Lz4Archive`](../) preparada para descomprimir.

```csharp
public Lz4Archive(Stream sourceStream, Lz4LoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | Flujo | La fuente del archivo. |
| loadOptions | Lz4LoadOptions | Las opciones con las que cargar el archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | No se puede leer de *sourceStream* |
| ArgumentNullException | *sourceStream* es nulo. |
| EndOfStreamException | *sourceStream* es demasiado corto. |
| InvalidDataException | El *sourceStream* tiene una firma incorrecta. |
| ObjectDisposedException | Se lanza si el flujo de origen ha sido eliminado. |
| IOException | Se produce un error de E/S. |

## Observaciones

Este constructor no descomprime. Consulte el método [`Open`](../open/) para descomprimir.

## Ejemplos

Abra un archivo desde un flujo y extráigalo a un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive(File.OpenRead("archive.lz4")))
  archive.Open().CopyTo(ms);
```

### Ver también

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(string, Lz4LoadOptions) {#constructor_2}

Inicializa una nueva instancia de la clase [`Lz4Archive`](../).

```csharp
public Lz4Archive(string path, Lz4LoadOptions loadOptions = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta al archivo de archivo. |
| loadOptions | Lz4LoadOptions | Las opciones con las que cargar el archivo. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *path* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder |
| ArgumentException | La *path* está vacía, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *path* denegado. |
| PathTooLongException | La *path* especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *path* contiene dos puntos (:) en medio de la cadena. |
| EndOfStreamException | El archivo es demasiado corto. |
| InvalidDataException | Los datos en el archivo tienen una firma incorrecta. |
| DirectoryNotFoundException | La ruta especificada no es válida, como por ejemplo estar en una unidad no asignada. |
| FileNotFoundException | El archivo no se encuentra. |
| IOException | El archivo ya está abierto. |

## Observaciones

Este constructor no descomprime. Consulte el método [`Open`](../open/) para descomprimir.

## Ejemplos

Abra un archivo desde la ruta del archivo y extráigalo a un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive("archive.lz4"))
  archive.Open().CopyTo(ms);
```

### Ver también

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(Lz4ArchiveSetting) {#constructor}

Inicializa una nueva instancia de la clase [`Lz4Archive`](../) preparada para comprimir.

```csharp
public Lz4Archive(Lz4ArchiveSetting settings = null)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| configuraciones | Lz4ArchiveSetting | La configuración del archivo compuesto. |

### Ver también

* class [Lz4ArchiveSetting](../../lz4archivesetting/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


