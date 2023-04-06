---
title: Bzip2CompressionSettings.Bzip2CompressionSettings
second_title: Aspose.ZIP for .NET API Referansı
description: Bzip2CompressionSettings inşaatçı. Yeni bir örneğini başlatır.Bzip2CompressionSettings sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

Yeni bir örneğini başlatır.[`Bzip2CompressionSettings`](../) sınıf.

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| blockSize | Int32 | Yüzlerce kilobayt cinsinden blok boyutu. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentOutOfRangeException | Blok boyutu 1 ile 9 arasında değildir. |

### Örnekler

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Ayrıca bakınız

* class [Bzip2CompressionSettings](../)
* ad alanı [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* toplantı [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

Yeni bir örneğini başlatır.[`Bzip2CompressionSettings`](../) varsayılan blok boyutuna sahip sınıf, 9 yüz kilobayta eşittir.

```csharp
public Bzip2CompressionSettings()
```

### Örnekler

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Ayrıca bakınız

* class [Bzip2CompressionSettings](../)
* ad alanı [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* toplantı [Aspose.Zip](../../../)


