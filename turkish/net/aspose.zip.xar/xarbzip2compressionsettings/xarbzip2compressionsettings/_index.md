---
title: "XarBzip2CompressionSettings.XarBzip2CompressionSettings"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "XarBzip2CompressionSettings yapıcı. XarBzip2CompressionSettings sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

[`XarBzip2CompressionSettings`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public XarBzip2CompressionSettings(int blockSize)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| blockSize | Int32 | Blok boyutu, yüz kilobayt cinsindendir. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentOutOfRangeException | Blok boyutu 1 ile 9 arasında değil. |

## Örnekler

```csharp
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### Ayrıca Bakınız

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

[`XarBzip2CompressionSettings`](../) sınıfının yeni bir örneğini varsayılan blok boyutuyla başlatır; bu, 9 yüz kilobyte eder.

```csharp
public XarBzip2CompressionSettings()
```

### Ayrıca Bakınız

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


