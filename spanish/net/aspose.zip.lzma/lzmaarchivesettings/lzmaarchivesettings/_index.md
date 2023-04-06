---
title: LzmaArchiveSettings.LzmaArchiveSettings
second_title: Referencia de la API de Aspose.ZIP para .NET
description: LzmaArchiveSettings constructor. Inicializa una nueva instancia delLzmaArchiveSettingsclase con tamaño de diccionario predeterminado igual a 16 megabytes.
type: docs
weight: 10
url: /es/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

Inicializa una nueva instancia del[`LzmaArchiveSettings`](../)clase con tamaño de diccionario predeterminado, igual a 16 megabytes.

```csharp
public LzmaArchiveSettings()
```

### Ejemplos

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 } )
{
    archive.SetSource("data.bin);
    archive.Save(lzmaFile);
}
```

### Ver también

* class [LzmaArchiveSettings](../)
* espacio de nombres [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* asamblea [Aspose.Zip](../../../)


