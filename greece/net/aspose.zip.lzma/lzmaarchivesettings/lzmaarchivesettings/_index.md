---
title: "LzmaArchiveSettings.LzmaArchiveSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής LzmaArchiveSettings. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης LzmaArchiveSettings με προεπιλεγμένο μέγεθος λεξικού ίσο με 16 megabytes, αριθμό γρήγορων byte ίσο με 32 και bits κυριολεκτικού πλαισίου ίσα με 3"
type: docs
weight: 10
url: /el/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`LzmaArchiveSettings`](../) με προεπιλεγμένο μέγεθος λεξικού ίσο με 16 megabytes, αριθμό γρήγορων byte ίσο με 32 και bits κυριολεκτικού πλαισίου ίσα με 3.

```csharp
public LzmaArchiveSettings()
```

## Παραδείγματα

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 })
{
    archive.SetSource("data.bin");
    archive.Save(lzmaFile);
}
```

### Δείτε επίσης

* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


