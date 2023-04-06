---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: DeflateCompressionSettings costruttore. Inizializza una nuova istanza diDeflateCompressionSettings classe.
type: docs
weight: 10
url: /it/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

Inizializza una nuova istanza di[`DeflateCompressionSettings`](../) classe.

```csharp
public DeflateCompressionSettings()
```

### Esempi

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Guarda anche

* class [DeflateCompressionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* assemblea [Aspose.Zip](../../../)


