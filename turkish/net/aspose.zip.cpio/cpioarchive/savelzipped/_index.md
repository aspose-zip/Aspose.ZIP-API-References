---
title: "CpioArchive.SaveLzipped"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "CpioArchive yöntemi. Arşivi lzip sıkıştırmasıyla akışa kaydeder"
type: docs
weight: 100
url: /tr/net/aspose.zip.cpio/cpioarchive/savelzipped/
---
## SaveLzipped(Stream, CpioFormat) {#savelzipped}

Arşivi lzip sıkıştırmasıyla akışa kaydeder.

```csharp
public void SaveLzipped(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| çıktı | Akış | Hedef akış. |
| cpioFormat | CpioFormat | cpio başlık formatını tanımlar. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *output* null. |
| ArgumentException | *output* yazılabilir değil. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |

## Açıklamalar

*output* must be writable.

## Örnekler

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### Ayrıca Bakınız

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLzipped(string, CpioFormat) {#savelzipped_1}

Arşivi lzip sıkıştırmasıyla yol belirterek dosyaya kaydeder.

```csharp
public void SaveLzipped(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacak. |
| cpioFormat | CpioFormat | cpio başlık formatını tanımlar. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| ArgumentException | *path* sıfır uzunlukta bir dizedir, yalnızca boşluk içerir veya InvalidPathChars tarafından tanımlanan bir veya daha fazla geçersiz karakter içerir. |
| ArgumentNullException | *path* `null`. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, (örneğin, eşlenmemiş bir sürücüde bulunması). |
| IOException | Bir G/Ç hatası oluştu. |
| PathTooLongException | Belirtilen yol, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşar. |
| UnauthorizedAccessException | Çağıran gerekli izne sahip değil. -veya- *path* salt okunur bir dosya veya dizin belirtti. |

## Örnekler

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.cpio.lz");
    }
}
```

### Ayrıca Bakınız

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


