---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: Aspose.ZIP for .NET API Referansı
description: SevenZipPPMdCompressionSettings inşaatçı. 7z arşivi içinde PPMd sıkıştırma yöntemi için ayarları somutlaştırır.
type: docs
weight: 10
url: /tr/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

7z arşivi içinde PPMd sıkıştırma yöntemi için ayarları somutlaştırır.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| maxOrder | Byte | Maksimum sipariş. |
| suballocatorSize | Int32 | MB alt ayırıcıdaki bellek boyutu tüketebilir. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* 2 ile 32 arasında değil veya*suballocatorSize* 1 ile 1024 arasında değil. |

### Notlar

Daha büyük model siparişleri neredeyse kesinlikle daha iyi sıkıştırma ve kesinlikle daha fazla bellek ve CPU kullanımı ile sonuçlanır.

PPMd algoritması, özellikle büyük dosyalarda kullanıldığında ve/veya büyük model düzeniyle kullanıldığında çok fazla belleğe ihtiyaç duyabilir. Eğer ppmd, verdiğinizden daha fazla belleğe ihtiyaç duyarsa, sıkıştırma daha kötü olacaktır.

### Örnekler

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Ayrıca bakınız

* class [SevenZipPPMdCompressionSettings](../)
* ad alanı [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* toplantı [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

Varsayılan model sırası ve alt ayırıcı boyutuyla 7z arşivi içinde PPMd sıkıştırma yöntemi ayarlarını somutlaştırır.

```csharp
public SevenZipPPMdCompressionSettings()
```

### Notlar

Varsayılan model sırası 6'dır ve alt ayırıcı boyutu 16MB'dir.

### Örnekler

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Ayrıca bakınız

* class [SevenZipPPMdCompressionSettings](../)
* ad alanı [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* toplantı [Aspose.Zip](../../../)


