---
title: LzmaArchiveSettings.LzmaArchiveSettings
second_title: Aspose.ZIP för .NET API-referens
description: LzmaArchiveSettings byggare. Initierar en ny instans avLzmaArchiveSettingsklass med standardstorlek för ordbok lika med 16 megabyte.
type: docs
weight: 10
url: /sv/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

Initierar en ny instans av[`LzmaArchiveSettings`](../)klass med standardstorlek för ordbok, lika med 16 megabyte.

```csharp
public LzmaArchiveSettings()
```

### Exempel

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 } )
{
    archive.SetSource("data.bin);
    archive.Save(lzmaFile);
}
```

### Se även

* class [LzmaArchiveSettings](../)
* namnutrymme [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* hopsättning [Aspose.Zip](../../../)


