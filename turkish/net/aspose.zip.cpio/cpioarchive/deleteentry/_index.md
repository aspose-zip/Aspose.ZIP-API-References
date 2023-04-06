---
title: CpioArchive.DeleteEntry
second_title: Aspose.ZIP for .NET API Referansı
description: CpioArchive yöntem. Belirli bir girişin ilk örneğini girişler listesinden kaldırır.
type: docs
weight: 50
url: /tr/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

Belirli bir girişin ilk örneğini girişler listesinden kaldırır.

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| entry | CpioEntry | Girişler listesinden kaldırılacak giriş. |

### Geri dönüş değeri

Cpio giriş örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *entry* boş. |

### Örnekler

Sonuncusu dışındaki tüm girişleri şu şekilde kaldırabilirsiniz:

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### Ayrıca bakınız

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* ad alanı [Aspose.Zip.Cpio](../../cpioarchive/)
* toplantı [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Girişi index. ile girişler listesinden kaldırır.

```csharp
public CpioArchive DeleteEntry(int entryIndex)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| entryIndex | Int32 | Kaldırılacak girişin sıfır tabanlı dizini. |

### Geri dönüş değeri

Girişin silindiği arşiv.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* 0.-veya-'den küçüktür*entryIndex* eşit veya daha büyük`Girdileri` saymak. |

### Örnekler

```csharp
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### Ayrıca bakınız

* class [CpioArchive](../)
* ad alanı [Aspose.Zip.Cpio](../../cpioarchive/)
* toplantı [Aspose.Zip](../../../)


