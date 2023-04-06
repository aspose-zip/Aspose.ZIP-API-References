---
title: StoreCompressionSettings.StoreCompressionSettings
second_title: Referencia de la API de Aspose.ZIP para .NET
description: StoreCompressionSettings constructor. Inicializa una nueva instancia delStoreCompressionSettings clase.
type: docs
weight: 10
url: /es/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

Inicializa una nueva instancia del[`StoreCompressionSettings`](../) clase.

```csharp
public StoreCompressionSettings()
```

### Ejemplos

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Ver también

* class [StoreCompressionSettings](../)
* espacio de nombres [Aspose.Zip.Saving](../../storecompressionsettings/)
* asamblea [Aspose.Zip](../../../)


