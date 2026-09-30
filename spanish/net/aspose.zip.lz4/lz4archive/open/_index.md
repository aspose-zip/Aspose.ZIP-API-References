---
title: "Lz4Archive.Open"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Método Lz4Archive. Abre el archivo para extracción y proporciona un flujo con el contenido del archivo."
type: docs
weight: 50
url: /es/net/aspose.zip.lz4/lz4archive/open/
---
## Lz4Archive.Open method

Abre el archivo para extracción y proporciona un flujo con el contenido del archivo.

```csharp
public Stream Open()
```

### Valor devuelto

El flujo que representa el contenido del archivo.

### Excepciones

| excepción | condición |
| --- | --- |
| EndOfStreamException | El flujo de origen es demasiado corto. |
| InvalidDataException | Se encontraron bytes incorrectos al iniciar la decodificación. |
| InvalidOperationException | El archivo está preparado para la composición. |
| ObjectDisposedException | El archivo ha sido eliminado y no se puede usar. |
| IOException | Se produce un error de E/S. |

## Observaciones

Lea del flujo para obtener el contenido original de un archivo. Consulte la sección de ejemplos.

## Ejemplos

Extrae el archivo y copia el contenido extraído al flujo de archivo.

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
    using (var extracted = File.Create("data.bin"))
    {
        var unpacked = archive.Open();
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }            
}
```

Puede usar el método Stream.CopyTo para .NET 4.0 o superior:

```csharp
unpacked.CopyTo(extracted);
```

### Ver también

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


