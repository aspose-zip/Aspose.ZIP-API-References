---
title: CpioArchive.SaveXzCompressed
second_title: Referencia de la API de Aspose.ZIP para .NET
description: CpioArchive método. Guarda el archivo en la secuencia con compresión xz.
type: docs
weight: 100
url: /es/net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## SaveXzCompressed(Stream, CpioFormat, XzArchiveSettings) {#savexzcompressed}

Guarda el archivo en la secuencia con compresión xz.

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| output | Stream | Flujo de destino. |
| cpioFormat | CpioFormat | Define el formato del encabezado cpio. |
| settings | XzArchiveSettings | Conjunto de configuración de archivo xz particular: tamaño de diccionario, tamaño de bloque, tipo de verificación. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *output* es nulo. |
| ArgumentException | *output* no se puede escribir. |

### Observaciones

*output*La secuencia debe ser escribible.

### Ejemplos

```csharp
using (FileStream result = File.OpenWrite("result.cpio.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### Ver también

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* espacio de nombres [Aspose.Zip.Cpio](../../cpioarchive/)
* asamblea [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, CpioFormat, XzArchiveSettings) {#savexzcompressed_1}

Guarda el archivo en ruta por ruta con compresión xz.

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | La ruta del archivo que se va a crear. Si el nombre de archivo especificado apunta a un archivo existente, se sobrescribirá. |
| cpioFormat | CpioFormat | Define el formato del encabezado cpio. |
| settings | XzArchiveSettings | Conjunto de configuración de archivo xz particular: tamaño de diccionario, tamaño de bloque, tipo de verificación. |

### Ejemplos

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.cpio.xz");
    }
}
```

### Ver también

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* espacio de nombres [Aspose.Zip.Cpio](../../cpioarchive/)
* asamblea [Aspose.Zip](../../../)


