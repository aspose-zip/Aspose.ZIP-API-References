---
title: "CpioArchive.SaveZCompressed"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método CpioArchive. Guarda el archivo en el flujo con compresión Z."
type: docs
weight: 130
url: /es/net/aspose.zip.cpio/cpioarchive/savezcompressed/
---
## SaveZCompressed(Stream, CpioFormat) {#savezcompressed}

Guarda el archivo en el flujo con compresión Z.

```csharp
public void SaveZCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
using (FileStream result = File.OpenWrite("result.cpio.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
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

## SaveZCompressed(string, CpioFormat) {#savezcompressed_1}

Guarda el archivo en la ruta por ruta con compresión Z.

```csharp
public void SaveZCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
| DirectoryNotFoundException | La ruta especificada no es válida, (por ejemplo, está en una unidad no asignada). |
| IOException | Se produce un error de E/S. |
| PathTooLongException | La ruta especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. |

## Ejemplos

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZCompressed("result.cpio.Z");
    }
}
```

### Ver también

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


