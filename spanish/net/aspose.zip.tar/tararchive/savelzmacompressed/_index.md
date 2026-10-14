---
title: "TarArchive.SaveLZMACompressed"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método TarArchive. Guarda el archivo en el flujo con compresión LZMA"
type: docs
weight: 190
url: /es/net/aspose.zip.tar/tararchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, TarFormat?) {#savelzmacompressed}

Guarda el archivo en el flujo con compresión LZMA.

```csharp
public void SaveLZMACompressed(Stream output, TarFormat? format = default)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| salida | Flujo | Flujo de destino. |
| formato | Nullable`1 | Define el formato de encabezado tar. El valor nulo se tratará como USTar cuando sea posible. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | *output* es nulo. |
| ArgumentException | *output* no es escribible. |
| ObjectDisposedException | El archivo ha sido descartado y no se puede usar |
| IOException | Se produce un error de E/S. |

## Observaciones

*output* must be writable.

Importante: el archivo tar se compone y luego se comprime dentro de este método, su contenido se mantiene internamente. Tenga cuidado con el consumo de memoria.

## Ejemplos

```csharp
using (FileStream result = File.OpenWrite("result.tar.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
        }
    }
}
```

### Ver también

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZMACompressed(string, TarFormat?) {#savelzmacompressed_1}

Guarda el archivo en el archivo mediante la ruta con compresión lzma.

```csharp
public void SaveLZMACompressed(string path, TarFormat? format = default)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | La ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito. |
| formato | Nullable`1 | Define el formato de encabezado tar. El valor nulo se tratará como USTar cuando sea posible. |

### Excepciones

| excepción | condición |
| --- | --- |
| UnauthorizedAccessException | El llamador no tiene el permiso requerido. -o- *path* especificó un archivo o directorio de solo lectura. |
| ArgumentException | *path* es una cadena de longitud cero, contiene solo espacios en blanco, o contiene uno o más caracteres no válidos según lo definido por InvalidPathChars. |
| ArgumentNullException | *path* es nulo. |
| PathTooLongException | La *path* especificada, el nombre de archivo, o ambos superan la longitud máxima definida por el sistema. Por ejemplo, en plataformas basadas en Windows, las rutas deben tener menos de 248 caracteres y los nombres de archivo menos de 260 caracteres. |
| DirectoryNotFoundException | La *path* especificada no es válida, (por ejemplo, está en una unidad no asignada). |
| NotSupportedException | *path* tiene un formato no válido. |
| ObjectDisposedException | El archivo ha sido descartado y no se puede usar |
| IOException | Se produce un error de E/S. |

## Observaciones

Importante: el archivo tar se compone y luego se comprime dentro de este método, su contenido se mantiene internamente. Tenga cuidado con el consumo de memoria.

## Ejemplos

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.tar.lzma");
    }
}
```

### Ver también

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


