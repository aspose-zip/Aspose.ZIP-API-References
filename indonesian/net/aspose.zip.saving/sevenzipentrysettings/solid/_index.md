---
title: "SevenZipEntrySettings.Solid"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti SevenZipEntrySettings. Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menggabungkan entri dan memperlakukannya sebagai satu blok data tunggal."
type: docs
weight: 50
url: /id/net/aspose.zip.saving/sevenzipentrysettings/solid/
---
## SevenZipEntrySettings.Solid property

Mendapatkan atau mengatur nilai yang menunjukkan apakah entri akan digabungkan dan diperlakukan sebagai satu blok data.

```csharp
public bool Solid { get; set; }
```

## Catatan

Sediakan `SevenZipEntrySettings` untuk arsip 7z solid saat pembuatan arsip.

## Contoh

Contoh berikut menunjukkan cara mengompres sebuah direktori menjadi arsip 7z solid dengan kompresi LZMA2 tanpa enkripsi.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings()){ Solid = true }))
    {
        archive.CreateEntries("C:\\Documents");
        archive.Save(sevenZipFile);
    }
}
```

### Lihat Juga

* class [SevenZipEntrySettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipentrysettings/)
* assembly [Aspose.Zip](../../../)


