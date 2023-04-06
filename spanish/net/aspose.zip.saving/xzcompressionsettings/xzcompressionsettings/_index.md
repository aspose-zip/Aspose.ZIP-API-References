---
title: XzCompressionSettings.XzCompressionSettings
second_title: Referencia de la API de Aspose.ZIP para .NET
description: XzCompressionSettings constructor. Inicializa una nueva instancia delXzCompressionSettings clase.
type: docs
weight: 10
url: /es/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

Inicializa una nueva instancia del[`XzCompressionSettings`](../) clase.

```csharp
public XzCompressionSettings()
```

### Ejemplos

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Ver también

* class [XzCompressionSettings](../)
* espacio de nombres [Aspose.Zip.Saving](../../xzcompressionsettings/)
* asamblea [Aspose.Zip](../../../)


