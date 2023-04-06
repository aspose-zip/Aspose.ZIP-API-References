---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: Referencia de la API de Aspose.ZIP para .NET
description: LzmaCompressionSettings constructor. Inicializa una nueva instancia delLzmaCompressionSettingsclase con tamaño de diccionario predeterminado igual a 16 megabytes.
type: docs
weight: 10
url: /es/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

Inicializa una nueva instancia del[`LzmaCompressionSettings`](../)clase con tamaño de diccionario predeterminado, igual a 16 megabytes.

```csharp
public LzmaCompressionSettings()
```

### Ejemplos

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Ver también

* class [LzmaCompressionSettings](../)
* espacio de nombres [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* asamblea [Aspose.Zip](../../../)


