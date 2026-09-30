---
title: "CpioArchive.SaveZstandard"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método CpioArchive. Guarda el archivo en el flujo con compresión Zstandard."
type: docs
weight: 140
url: /es/net/aspose.zip.cpio/cpioarchive/savezstandard/
---
## SaveZstandard(Stream, CpioFormat) {#savezstandard}

Guarda el archivo en el flujo con compresión Zstandard.

```csharp
public void SaveZstandard(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| salida | Flujo | Flujo de destino. |
| cpioFormat | CpioFormat | Define el formato de encabezado cpio. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *output* es nulo. |
| ArgumentException | *output* no es escribible. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |

## Observaciones

*output* must be writable.

## Ejemplos

```csharp
using (FileStream result = File.OpenWrite("result.cpio.zst"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZstandard(result);
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

## SaveZstandard(string, CpioFormat) {#savezstandard_1}

Guarda el archivo en el archivo por ruta con compresión Zstandard.

```csharp
public void SaveZstandard(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito. |
| cpioFormat | CpioFormat | Define el formato de encabezado cpio. |

### Excepciones

| excepción | condición |
| --- | --- |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| ArgumentException | *path* es una cadena de longitud cero, contiene solo espacios en blanco, o contiene uno o más caracteres no válidos según lo definido por InvalidPathChars. |
| ArgumentNullException | *path* es `null`. |
| DirectoryNotFoundException | La ruta especificada no es válida, (por ejemplo, está en una unidad no asignada). |
| IOException | Se produce un error de E/S. |
| PathTooLongException | La ruta especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. |
| UnauthorizedAccessException | El llamador no tiene el permiso requerido. -o- *path* especificó un archivo o directorio de solo lectura. |

## Ejemplos

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZstandard("result.cpio.zst");
    }
}
```

### Ver también

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


