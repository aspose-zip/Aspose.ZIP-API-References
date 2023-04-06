---
title: LzmaArchiveSettings.LzmaArchiveSettings
second_title: Aspose.ZIP für .NET-API-Referenz
description: LzmaArchiveSettings constructeur. Initialisiert eine neue Instanz vonLzmaArchiveSettingsKlasse mit Standardwörterbuchgröße entspricht 16 Megabyte.
type: docs
weight: 10
url: /de/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

Initialisiert eine neue Instanz von[`LzmaArchiveSettings`](../)Klasse mit Standardwörterbuchgröße, entspricht 16 Megabyte.

```csharp
public LzmaArchiveSettings()
```

### Beispiele

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 } )
{
    archive.SetSource("data.bin);
    archive.Save(lzmaFile);
}
```

### Siehe auch

* class [LzmaArchiveSettings](../)
* namensraum [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* Montage [Aspose.Zip](../../../)


