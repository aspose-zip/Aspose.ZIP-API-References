---
title: "CpioArchive.SaveLZMACompressed"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método CpioArchive. Guarda el archivo en el flujo con compresión LZMA."
type: docs
weight: 110
url: /es/net/aspose.zip.cpio/cpioarchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, CpioFormat) {#savelzmacompressed}

Guarda el archivo en el flujo con compresión LZMA.

```csharp
public void SaveLZMACompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| salida | Flujo | Flujo de destino. |
| cpioFormat | CpioFormat | Define el formato de encabezado cpio. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| NotSupportedException | El flujo no admite escritura, o el flujo ya está cerrado. |

## Observaciones

*output* must be writable.

Importante: el archivo cpio se compone y luego se comprime dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

## Ejemplos

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
        }
    }
}
```

### Ver también

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZMACompressed(string, CpioFormat) {#savelzmacompressed_1}

Guarda el archivo en el archivo por ruta con compresión lzma.

```csharp
public void SaveLZMACompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito. |
| cpioFormat | CpioFormat | Define el formato de encabezado cpio. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| ArgumentNullException | *path* es `null`. |
| Excepción | Lanzada cuando ocurre un error de tiempo de ejecución. |
| DirectoryNotFoundException | La ruta especificada no es válida, (por ejemplo, está en una unidad no asignada). |
| IOException | Se produce un error de E/S. |
| PathTooLongException | La ruta especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. |
| UnauthorizedAccessException | El llamador no tiene el permiso requerido. -o- *path* especificó un archivo o directorio de solo lectura. |

## Observaciones

Importante: el archivo cpio se compone y luego se comprime dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

## Ejemplos

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.cpio.lzma");
    }
}
```

### Ver también

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


