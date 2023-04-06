---
title: LzmaArchiveSettings.LzmaArchiveSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: LzmaArchiveSettings costruttore. Inizializza una nuova istanza diLzmaArchiveSettingsclass con dimensione del dizionario predefinita pari a 16 megabyte.
type: docs
weight: 10
url: /it/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

Inizializza una nuova istanza di[`LzmaArchiveSettings`](../)class con dimensione del dizionario predefinita, pari a 16 megabyte.

```csharp
public LzmaArchiveSettings()
```

### Esempi

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 } )
{
    archive.SetSource("data.bin);
    archive.Save(lzmaFile);
}
```

### Guarda anche

* class [LzmaArchiveSettings](../)
* spazio dei nomi [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assemblea [Aspose.Zip](../../../)


