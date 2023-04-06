---
title: TarArchive.SaveXzCompressed
second_title: Referencia de la API de Aspose.ZIP para .NET
description: TarArchive método. Guarda el archivo en la secuencia con compresión xz.
type: docs
weight: 150
url: /es/net/aspose.zip.tar/tararchive/savexzcompressed/
---
## SaveXzCompressed(Stream, TarFormat?, XzArchiveSettings) {#savexzcompressed}

Guarda el archivo en la secuencia con compresión xz.

```csharp
public void SaveXzCompressed(Stream output, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| output | Stream | Flujo de destino. |
| format | Nullable`1 | Define el formato del encabezado tar. El valor nulo se tratará como UStar cuando sea posible. |
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
using (FileStream result = File.OpenWrite("result.tar.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### Ver también

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, TarFormat?, XzArchiveSettings) {#savexzcompressed_1}

Guarda el archivo en ruta por ruta con compresión xz.

```csharp
public void SaveXzCompressed(string path, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | La ruta del archivo que se va a crear. Si el nombre de archivo especificado apunta a un archivo existente, se sobrescribirá. |
| format | Nullable`1 | Define el formato del encabezado tar. El valor nulo se tratará como UStar cuando sea posible. |
| settings | XzArchiveSettings | Conjunto de configuración de archivo xz particular: tamaño de diccionario, tamaño de bloque, tipo de verificación. |

### Ejemplos

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.tar.xz");
    }
}
```

### Ver también

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)


