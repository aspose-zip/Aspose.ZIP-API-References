---
title: StoreCompressionSettings.StoreCompressionSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: StoreCompressionSettings costruttore. Inizializza una nuova istanza diStoreCompressionSettings classe.
type: docs
weight: 10
url: /it/net/aspose.zip.saving/storecompressionsettings/storecompressionsettings/
---
## StoreCompressionSettings constructor

Inizializza una nuova istanza di[`StoreCompressionSettings`](../) classe.

```csharp
public StoreCompressionSettings()
```

### Esempi

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Guarda anche

* class [StoreCompressionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../storecompressionsettings/)
* assemblea [Aspose.Zip](../../../)


