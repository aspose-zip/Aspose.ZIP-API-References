---
title: "XzCompressionSettings.XzCompressionSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor XzCompressionSettings. Menginisialisasi instance baru dari kelas XzCompressionSettings"
type: docs
weight: 10
url: /id/net/aspose.zip.saving/xzcompressionsettings/xzcompressionsettings/
---
## XzCompressionSettings constructor

Menginisialisasi instance baru dari kelas [`XzCompressionSettings`](../).

```csharp
public XzCompressionSettings()
```

## Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Lihat Juga

* class [XzCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../xzcompressionsettings/)
* assembly [Aspose.Zip](../../../)


