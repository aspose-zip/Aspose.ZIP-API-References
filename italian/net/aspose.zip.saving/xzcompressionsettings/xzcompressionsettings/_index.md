---
title: XzCompressionSettings.XzCompressionSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: XzCompressionSettings costruttore. Inizializza una nuova istanza diXzCompressionSettings classe.
type: docs
weight: 10
url: /it/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

Inizializza una nuova istanza di[`XzCompressionSettings`](../) classe.

```csharp
public XzCompressionSettings()
```

### Esempi

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Guarda anche

* class [XzCompressionSettings](../)
* spazio dei nomi [Aspose.Zip.Saving](../../xzcompressionsettings/)
* assemblea [Aspose.Zip](../../../)


