---
title: TarArchive.SaveZCompressed
second_title: Aspose.ZIP for .NET API Referansı
description: TarArchive yöntem. Arşivi Z sıkıştırmasıyla akışa kaydeder.
type: docs
weight: 160
url: /tr/net/aspose.zip.tar/tararchive/savezcompressed/
---
## SaveZCompressed(Stream, TarFormat?) {#savezcompressed}

Arşivi Z sıkıştırmasıyla akışa kaydeder.

```csharp
public void SaveZCompressed(Stream output, TarFormat? format = default)
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
using (FileStream result = File.OpenWrite("result.tar.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
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

## SaveZCompressed(string, TarFormat?) {#savezcompressed_1}

Z sıkıştırması ile arşivi yola göre yola kaydeder.

```csharp
public void SaveZCompressed(string path, TarFormat? format = default)
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
        archive.SaveZCompressed("result.tar.Z");
    }
}
```

### Ayrıca bakınız

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)


