---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: LzmaCompressionSettings costruttore. Inizializza una nuova istanza diLzmaCompressionSettingsclass con dimensione del dizionario predefinita pari a 16 megabyte.
type: docs
weight: 10
url: /it/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

Inizializza una nuova istanza di[`LzmaCompressionSettings`](../)class con dimensione del dizionario predefinita, pari a 16 megabyte.

```csharp
public LzmaCompressionSettings()
```

### Esempi

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Guarda anche

* class [LzmaCompressionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assemblea [Aspose.Zip](../../../)


