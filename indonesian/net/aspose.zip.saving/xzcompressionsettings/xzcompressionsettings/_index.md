---
title: XzCompressionSettings.XzCompressionSettings
second_title: Aspose.ZIP untuk Referensi .NET API
description: XzCompressionSettings konstruktor. Menginisialisasi instance baru dariXzCompressionSettings kelas.
type: docs
weight: 10
url: /id/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

Menginisialisasi instance baru dari[`XzCompressionSettings`](../) kelas.

```csharp
public XzCompressionSettings()
```

### Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Lihat juga

* class [XzCompressionSettings](../)
* ruang nama [Aspose.Zip.Saving](../../xzcompressionsettings/)
* perakitan [Aspose.Zip](../../../)


