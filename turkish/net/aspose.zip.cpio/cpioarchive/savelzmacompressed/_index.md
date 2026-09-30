---
title: "CpioArchive.SaveLZMACompressed"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "CpioArchive yöntemi. Arşivi LZMA sıkıştırmasıyla akışa kaydeder."
type: docs
weight: 110
url: /tr/net/aspose.zip.cpio/cpioarchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, CpioFormat) {#savelzmacompressed}

Arşivi LZMA sıkıştırmasıyla akışa kaydeder.

```csharp
public void SaveLZMACompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| çıktı | Akış | Hedef akış. |
| cpioFormat | CpioFormat | cpio başlık formatını tanımlar. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| NotSupportedException | Akış yazmayı desteklemiyor veya akış zaten kapalı. |

## Açıklamalar

*output* must be writable.

Önemli: cpio arşivi bu yöntem içinde oluşturulur ve ardından sıkıştırılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

## Örnekler

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
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

## SaveLZMACompressed(string, CpioFormat) {#savelzmacompressed_1}

Arşivi lzma sıkıştırmasıyla yol belirterek dosyaya kaydeder.

```csharp
public void SaveLZMACompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacak. |
| cpioFormat | CpioFormat | cpio başlık formatını tanımlar. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz. |
| ArgumentNullException | *path* `null`. |
| İstisna | Çalışma zamanı hatası oluştuğunda atılır. |
| DirectoryNotFoundException | Belirtilen yol geçersiz, (örneğin, eşlenmemiş bir sürücüde bulunması). |
| IOException | Bir G/Ç hatası oluştu. |
| PathTooLongException | Belirtilen yol, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşar. |
| UnauthorizedAccessException | Çağıran gerekli izne sahip değil. -veya- *path* salt okunur bir dosya veya dizin belirtti. |

## Açıklamalar

Önemli: cpio arşivi bu yöntem içinde oluşturulur ve ardından sıkıştırılır, içeriği dahili olarak tutulur. Bellek tüketimine dikkat edin.

## Örnekler

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.cpio.lzma");
    }
}
```

### Ayrıca Bakınız

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


