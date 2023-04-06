---
title: XzArchiveSettings.XzArchiveSettings
second_title: Aspose.ZIP for .NET API Referansı
description: XzArchiveSettings inşaatçı. Yeni bir örneğini başlatır.XzArchiveSettings tek LZMA2 sıkıştırması kullanan sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip.xz.settings/xzarchivesettings/xzarchivesettings/
---
## XzArchiveSettings() {#constructor}

Yeni bir örneğini başlatır.[`XzArchiveSettings`](../) tek LZMA2 sıkıştırması kullanan sınıf.

```csharp
public XzArchiveSettings()
```

### Notlar

LZMA2'deki varsayılan sözlük boyutu 16 megabayta eşittir, varsayılan blok boyutu 64 megabayta eşittir, varsayılan sağlama toplamı türü CRC32.

### Ayrıca bakınız

* class [XzArchiveSettings](../)
* ad alanı [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* toplantı [Aspose.Zip](../../../)

---

## XzArchiveSettings(XzFilterSettings[], long, XzCheckType) {#constructor_1}

Yeni bir örneğini başlatır.[`XzArchiveSettings`](../) özel parametrelerle sınıf.

```csharp
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filters | XzFilterSettings[] | Oluşturmak için sırayla uygulanacak filtreler (kompresörler)[`XzArchive`](../../../aspose.zip.xz/xzarchive/) . tek de olabilir[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) veya bir çift[`XzBcjX86FilterSettings`](../../xzbcjx86filtersettings/) Ve[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) |
| blockSize | Int64 | Boyut xz arşiv bloğu. |
| checkType | XzCheckType | Sıkıştırılmamış veriler için sağlama toplamı hesaplama türü. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentOutOfRangeException | *blockSize* olumsuz. |
| ArgumentNullException | *filters* boş |
| ArgumentException | *filters* birden az veya ikiden fazla filtreye sahip veya son filtre değil[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |

### Örnekler

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
    XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
    using (var archive = new XzArchive(settings))
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### Ayrıca bakınız

* class [XzFilterSettings](../../xzfiltersettings/)
* enum [XzCheckType](../../xzchecktype/)
* class [XzArchiveSettings](../)
* ad alanı [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* toplantı [Aspose.Zip](../../../)


