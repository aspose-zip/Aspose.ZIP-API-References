---
title: TarArchive.SaveLzipped
second_title: Aspose.ZIP for .NET API Referansı
description: TarArchive yöntem. Arşivi lzip sıkıştırmasıyla akışa kaydeder.
type: docs
weight: 140
url: /tr/net/aspose.zip.tar/tararchive/savelzipped/
---
## SaveLzipped(Stream, TarFormat?) {#savelzipped}

Arşivi lzip sıkıştırmasıyla akışa kaydeder.

```csharp
public void SaveLzipped(Stream output, TarFormat? format = default)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| output | Stream | Hedef akışı. |
| format | Nullable`1 | tar başlık biçimini tanımlar. Boş değer, mümkün olduğunda USar olarak ele alınacaktır. |

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *output* boş. |
| ArgumentException | *output* yazılabilir değil. |

### Notlar

*output*yazılabilir olmalıdır.

### Örnekler

```csharp
using (FileStream result = File.OpenWrite("result.tar.lz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### Ayrıca bakınız

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)

---

## SaveLzipped(string, TarFormat?) {#savelzipped_1}

Arşivi, lzip sıkıştırması ile yola göre dosyaya kaydeder.

```csharp
public void SaveLzipped(string path, TarFormat? format = default)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| path | String | Oluşturulacak arşivin yolu. Belirtilen dosya adı mevcut bir dosyaya işaret ediyorsa, üzerine yazılacaktır. |
| format | Nullable`1 | tar başlık biçimini tanımlar. Boş değer, mümkün olduğunda USar olarak ele alınacaktır. |

### Örnekler

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.tar.lz");
    }
}
```

### Ayrıca bakınız

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)


