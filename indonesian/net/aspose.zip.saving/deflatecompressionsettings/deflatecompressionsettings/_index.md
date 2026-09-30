---
title: "DeflateCompressionSettings.DeflateCompressionSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor DeflateCompressionSettings. Menginisialisasi sebuah instance baru dari kelas DeflateCompressionSettings"
type: docs
weight: 10
url: /id/net/aspose.zip.saving/deflatecompressionsettings/deflatecompressionsettings/
---
## DeflateCompressionSettings constructor

Menginisialisasi sebuah instance baru dari kelas [`DeflateCompressionSettings`](../).

```csharp
public DeflateCompressionSettings()
```

## Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Lihat Juga

* class [DeflateCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../deflatecompressionsettings/)
* assembly [Aspose.Zip](../../../)


