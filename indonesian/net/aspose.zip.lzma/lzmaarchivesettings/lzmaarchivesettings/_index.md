---
title: LzmaArchiveSettings.LzmaArchiveSettings
second_title: Aspose.ZIP untuk Referensi .NET API
description: LzmaArchiveSettings konstruktor. Menginisialisasi instance baru dariLzmaArchiveSettingskelas dengan ukuran kamus default sama dengan 16 megabyte.
type: docs
weight: 10
url: /id/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

Menginisialisasi instance baru dari[`LzmaArchiveSettings`](../)kelas dengan ukuran kamus default, sama dengan 16 megabyte.

```csharp
public LzmaArchiveSettings()
```

### Contoh

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 } )
{
    archive.SetSource("data.bin);
    archive.Save(lzmaFile);
}
```

### Lihat juga

* class [LzmaArchiveSettings](../)
* ruang nama [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* perakitan [Aspose.Zip](../../../)


