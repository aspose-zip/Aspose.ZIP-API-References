---
title: "SevenZipEntrySettings.Solid"
second_title: "Referencia de API de Aspose.ZIP para .NET"
description: "Propiedad SevenZipEntrySettings. Obtiene o establece el valor que indica si concatenar las entradas y tratarlas como un único bloque de datos"
type: docs
weight: 50
url: /es/net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

Obtiene o establece el valor que indica si se deben concatenar las entradas y tratarlas como un único bloque de datos.

```csharp
public bool Solid { get; set; }
```

## Observaciones

Proporcione `SevenZipEntrySettings` para un archivo 7z sólido al instanciar el archivo.

## Ejemplos

El siguiente ejemplo muestra cómo comprimir un directorio a un archivo 7z sólido con compresión LZMA2 sin cifrado.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings()){ Solid = true }))
    {
        archive.CreateEntries("C:\\Documents");
        archive.Save(sevenZipFile);
    }
}
```

### Ver también

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


