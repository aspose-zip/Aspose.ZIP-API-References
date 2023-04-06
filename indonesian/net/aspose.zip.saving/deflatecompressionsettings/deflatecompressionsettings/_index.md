---
title: DeflateCompressionSettings.DeflateCompressionSettings
second_title: Aspose.ZIP untuk Referensi .NET API
description: DeflateCompressionSettings konstruktor. Menginisialisasi instance baru dariDeflateCompressionSettings kelas.
type: docs
weight: 10
url: /id/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

Menginisialisasi instance baru dari[`DeflateCompressionSettings`](../) kelas.

```csharp
public DeflateCompressionSettings()
```

### Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Lihat juga

* class [DeflateCompressionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* perakitan [Aspose.Zip](../../../)


