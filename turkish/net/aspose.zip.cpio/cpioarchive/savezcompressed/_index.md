---
title: "CpioArchive.SaveZCompressed"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "CpioArchive yöntemi. Arşivi Z sıkıştırmasıyla akışa kaydeder."
type: docs
weight: 130
url: /tr/net/aspose.zip.cpio/cpioarchive/savezcompressed/
---
## SaveZCompressed(Stream, CpioFormat) {#savezcompressed}

Arşivi Z sıkıştırmasıyla akışa kaydeder.

```csharp
public void SaveZCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
using (FileStream result = File.OpenWrite("result.cpio.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
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

## SaveZCompressed(string, CpioFormat) {#savezcompressed_1}

Arşivi yoluna Z sıkıştırmasıyla kaydeder.

```csharp
public void SaveZCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
| DirectoryNotFoundException | Belirtilen yol geçersiz, (örneğin, eşlenmemiş bir sürücüde bulunması). |
| IOException | Bir G/Ç hatası oluştu. |
| PathTooLongException | Belirtilen yol, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşar. |

## Örnekler

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZCompressed("result.cpio.Z");
    }
}
```

### Ayrıca Bakınız

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


