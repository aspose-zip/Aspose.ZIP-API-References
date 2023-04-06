---
title: TarArchive.SaveGzipped
second_title: Referencia de la API de Aspose.ZIP para .NET
description: TarArchive método. Guarda el archivo en la transmisión con compresión gzip.
type: docs
weight: 130
url: /es/net/aspose.zip.tar/tararchive/savegzipped/
---
## SaveGzipped(Stream, TarFormat?) {#savegzipped}

Guarda el archivo en la transmisión con compresión gzip.

```csharp
public void SaveGzipped(Stream output, TarFormat? format = default)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| output | Stream | Flujo de destino. |
| format | Nullable`1 | Define el formato del encabezado tar. El valor nulo se tratará como UStar cuando sea posible. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *output* es nulo. |
| ArgumentException | *output* no se puede escribir. |

### Observaciones

*output*debe ser escribible.

### Ejemplos

```csharp
using (FileStream result = File.OpenWrite("result.tar.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### Ver también

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)

---

## SaveGzipped(string, TarFormat?) {#savegzipped_1}

Guarda el archivo en el archivo por ruta con compresión gzip.

```csharp
public void SaveGzipped(string path, TarFormat? format = default)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| path | String | La ruta del archivo que se va a crear. Si el nombre de archivo especificado apunta a un archivo existente, se sobrescribirá. |
| format | Nullable`1 | Define el formato del encabezado tar. El valor nulo se tratará como UStar cuando sea posible. |

### Ejemplos

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.tar.gz");
    }
}
```

### Ver también

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* espacio de nombres [Aspose.Zip.Tar](../../tararchive/)
* asamblea [Aspose.Zip](../../../)


