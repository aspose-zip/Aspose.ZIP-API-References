---
title: "LzxArchiveEntry.Extract"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método LzxArchiveEntry. Extrae la entrada del archivo Lzx a un sistema de archivos por ruta"
type: docs
weight: 80
url: /es/net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

Extrae la entrada del archivo Lzx a un sistema de archivos mediante la ruta.

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
| InvalidDataException | Desajuste de suma de verificación para encabezados o datos. - o - El archivo está corrupto. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |
| NotSupportedException | Método de compresión no válido. |
| ObjectDisposedException | Se lanza si el flujo de origen ha sido eliminado. |
| EndOfStreamException | Se lanza cuando se alcanza inesperadamente el final del flujo. |

## Ejemplos

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Ver también

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

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
| InvalidDataException | Desajuste de suma de verificación para encabezados o datos. - o - El archivo está corrupto. |
| ArgumentNullException | El flujo de destino es nulo. |
| NotSupportedException | Método de compresión no válido. |
| OperationCanceledException | En .NET Framework 4.0 y superiores: Se lanza cuando la extracción se cancela mediante el token de cancelación proporcionado. |
| ObjectDisposedException | Se lanza si el flujo de origen ha sido eliminado. |
| EndOfStreamException | Se lanza cuando se alcanza inesperadamente el final del flujo. |

### Ver también

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


