---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: Referencia de la API de Aspose.ZIP para .NET
description: DeflateCompressionSettings constructor. Inicializa una nueva instancia delDeflateCompressionSettings clase.
type: docs
weight: 10
url: /es/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

Inicializa una nueva instancia del[`DeflateCompressionSettings`](../) clase.

```csharp
public DeflateCompressionSettings()
```

### Ejemplos

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Ver también

* class [DeflateCompressionSettings](../)
* espacio de nombres [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* asamblea [Aspose.Zip](../../../)


