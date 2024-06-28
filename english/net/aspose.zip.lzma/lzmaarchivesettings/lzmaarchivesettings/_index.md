---
title: LzmaArchiveSettings.LzmaArchiveSettings
second_title: Aspose.ZIP for .NET API Reference
description: LzmaArchiveSettings constructor. Initializes a new instance of the LzmaArchiveSettings class with default dictionary size equals to 16 megabytes
type: docs
weight: 10
url: /net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

Initializes a new instance of the [`LzmaArchiveSettings`](../) class with default dictionary size, equals to 16 megabytes.

```csharp
public LzmaArchiveSettings()
```

## Examples

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 } )
{
    archive.SetSource("data.bin);
    archive.Save(lzmaFile);
}
```

### See Also

* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


