---
title: LzmaArchiveSettings.LzmaArchiveSettings
second_title: Aspose.ZIP voor .NET API-referentie
description: LzmaArchiveSettings constructeur. Initialiseert een nieuw exemplaar van hetLzmaArchiveSettingsklasse met standaard woordenboekgrootte gelijk aan 16 megabytes.
type: docs
weight: 10
url: /nl/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

Initialiseert een nieuw exemplaar van het[`LzmaArchiveSettings`](../)klasse met standaard woordenboekgrootte, gelijk aan 16 megabytes.

```csharp
public LzmaArchiveSettings()
```

### Voorbeelden

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 } )
{
    archive.SetSource("data.bin);
    archive.Save(lzmaFile);
}
```

### Zie ook

* class [LzmaArchiveSettings](../)
* naamruimte [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* montage [Aspose.Zip](../../../)


