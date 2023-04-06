---
title: LzmaCompressionSettings.LzmaCompressionSettings
second_title: Aspose.ZIP untuk Referensi .NET API
description: LzmaCompressionSettings konstruktor. Menginisialisasi instance baru dariLzmaCompressionSettingskelas dengan ukuran kamus default sama dengan 16 megabyte.
type: docs
weight: 10
url: /id/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings constructor

Menginisialisasi instance baru dari[`LzmaCompressionSettings`](../)kelas dengan ukuran kamus default, sama dengan 16 megabyte.

```csharp
public LzmaCompressionSettings()
```

### Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Lihat juga

* class [LzmaCompressionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* perakitan [Aspose.Zip](../../../)


