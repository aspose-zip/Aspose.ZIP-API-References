---
title: "TarArchive.SaveZstandard"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "TarArchive yöntemi. Arşivi Zstandard sıkıştırmasıyla akışa kaydeder"
type: docs
weight: 220
url: /tr/net/aspose.zip.tar/tararchive/savezstandard/
---
## SaveZstandard(Stream, TarFormat?) {#savezstandard}

Arşivi Zstandard sıkıştırmasıyla akışa kaydeder.

```csharp
public void SaveZstandard(Stream output, TarFormat? format = default)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| çıktı | Akış | Hedef akış. |
| biçim | Nullable`1 | Tar başlık formatını tanımlar. Boş değer mümkün olduğunda USTar olarak kabul edilir. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | *output* null. |
| ArgumentException | *output* yazılabilir değil. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz |
| IOException | Bir G/Ç hatası oluştu. |

## Açıklamalar

*output* must be writable.

## Örnekler

```csharp
using (FileStream result = File.OpenWrite("result.tar.zst"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZstandard(result);
        }
    }
}
```

### Ayrıca Bakınız

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveZstandard(string, TarFormat?) {#savezstandard_1}

Arşivi, Zstandard sıkıştırmasıyla belirtilen yola kaydeder.

```csharp
public void SaveZstandard(string path, TarFormat? format = default)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yol | String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacak. |
| biçim | Nullable`1 | Tar başlık formatını tanımlar. Boş değer mümkün olduğunda USTar olarak kabul edilir. |

### İstisnalar

| istisna | koşul |
| --- | --- |
| UnauthorizedAccessException | Çağıran gerekli izne sahip değil. -veya- *path* salt okunur bir dosya veya dizin belirtti. |
| ArgumentException | *path* sıfır uzunlukta bir dizedir, yalnızca boşluk içerir veya InvalidPathChars tarafından tanımlanan bir veya daha fazla geçersiz karakter içerir. |
| ArgumentNullException | *path* null. |
| PathTooLongException | Belirtilen *path*, dosya adı veya her ikisi sistem tarafından tanımlanan maksimum uzunluğu aşıyor. Örneğin, Windows tabanlı platformlarda yollar 248 karakterden, dosya adları ise 260 karakterden kısa olmalıdır. |
| DirectoryNotFoundException | Belirtilen *path* geçersizdir (örneğin, eşlenmemiş bir sürücüde). |
| NotSupportedException | *path* geçersiz bir biçimde. |
| ObjectDisposedException | Arşiv serbest bırakıldı ve kullanılamaz |

## Örnekler

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZstandard("result.tar.zst");
    }
}
```

### Ayrıca Bakınız

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


