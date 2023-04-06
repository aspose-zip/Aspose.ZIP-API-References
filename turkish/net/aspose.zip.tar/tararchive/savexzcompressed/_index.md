---
title: TarArchive.SaveXzCompressed
second_title: Aspose.ZIP for .NET API Referansı
description: TarArchive yöntem. Arşivi xz sıkıştırmasıyla akışa kaydeder.
type: docs
weight: 150
url: /tr/net/aspose.zip.tar/tararchive/savexzcompressed/
---
## SaveXzCompressed(Stream, TarFormat?, XzArchiveSettings) {#savexzcompressed}

Arşivi xz sıkıştırmasıyla akışa kaydeder.

```csharp
public void SaveXzCompressed(Stream output, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| output | Stream | Hedef akışı. |
| format | Nullable`1 | tar başlık biçimini tanımlar. Boş değer, mümkün olduğunda USar olarak ele alınacaktır. |
| settings | XzArchiveSettings | Belirli xz arşivi ayar kümesi: sözlük boyutu, blok boyutu, kontrol tipi. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *output* boş. |
| ArgumentException | *output* yazılabilir değil. |

### Notlar

*output*Akış yazılabilir olmalıdır.

### Örnekler

```csharp
using (FileStream result = File.OpenWrite("result.tar.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### Ayrıca bakınız

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, TarFormat?, XzArchiveSettings) {#savexzcompressed_1}

Arşivi xz sıkıştırma ile yola göre yola kaydeder.

```csharp
public void SaveXzCompressed(string path, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |
| format | Nullable`1 | tar başlık biçimini tanımlar. Boş değer, mümkün olduğunda USar olarak ele alınacaktır. |
| settings | XzArchiveSettings | Belirli xz arşivi ayar kümesi: sözlük boyutu, blok boyutu, kontrol tipi. |

### Örnekler

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.tar.xz");
    }
}
```

### Ayrıca bakınız

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)


