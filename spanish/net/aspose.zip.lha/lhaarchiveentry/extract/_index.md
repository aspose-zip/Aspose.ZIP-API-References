---
title: "LhaArchiveEntry.Extract"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método LhaArchiveEntry. Extrae la entrada del archivo Lha a un sistema de archivos por ruta"
type: docs
weight: 60
url: /es/net/aspose.zip.lha/lhaarchiveentry/extract/
---
## Extract(string) {#extract}

Extrae la entrada del archivo Lha a un sistema de archivos mediante la ruta.

```csharp
public FileSystemInfo Extract(string path)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | Ruta al archivo que almacenará los datos descomprimidos. |

### Valor devuelto

FileSystemInfoInstance que contiene los datos extraídos.

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | No se leyeron los encabezados del archivo y la información del servicio. |
| ArgumentNullException | *path* es nulo. |
| SecurityException | El llamador no tiene el permiso requerido para acceder. |
| ArgumentException | La *path* está vacía, contiene solo espacios en blanco o contiene caracteres no válidos. |
| UnauthorizedAccessException | Acceso al archivo *path* denegado. |
| PathTooLongException | La *path* especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| NotSupportedException | El archivo en *path* contiene dos puntos (:) en medio de la cadena. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |
| ObjectDisposedException | Se lanza si el flujo de origen ha sido eliminado. |
| InvalidDataException | Se lanza cuando los datos son inválidos o están corruptos. |

## Ejemplos

```csharp
using (FileStream lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Ver también

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

Extrae la entrada al flujo proporcionado.

```csharp
public void Extract(Stream destination)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | Flujo | Secuencia de destino. Debe ser escribible. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | *destination* no admite escritura. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |
| ObjectDisposedException | Se lanza si el flujo de origen ha sido eliminado. |
| InvalidDataException | Se lanza cuando los datos son inválidos o están corruptos. |

## Observaciones

No hace nada para la entrada de directorio.

### Ver también

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Extrae la entrada del archivo Lha a un archivo.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo para almacenar datos descomprimidos. |

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | No se leyeron los encabezados del archivo y la información del servicio. |
| SecurityException | El llamador no tiene el permiso requerido para abrir el *fileInfo*. |
| ArgumentException | La ruta del archivo está vacía o contiene solo espacios en blanco. |
| FileNotFoundException | El archivo no se encuentra. |
| UnauthorizedAccessException | La ruta al archivo es de solo lectura o es un directorio. |
| ArgumentNullException | *fileInfo* es nulo. |
| DirectoryNotFoundException | La ruta especificada no es válida, como por ejemplo estar en una unidad no asignada. |
| IOException | El archivo ya está abierto. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |
| ObjectDisposedException | Se lanza si el flujo de origen ha sido eliminado. |

## Observaciones

No hace nada para la entrada de directorio.

## Ejemplos

```csharp
using (var lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Ver también

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)


