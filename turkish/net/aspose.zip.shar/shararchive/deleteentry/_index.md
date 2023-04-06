---
title: SharArchive.DeleteEntry
second_title: Aspose.ZIP for .NET API Referansı
description: SharArchive yöntem. Belirli bir girişin ilk örneğini girişler listesinden kaldırır.
type: docs
weight: 50
url: /tr/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

Belirli bir girişin ilk örneğini girişler listesinden kaldırır.

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| entry | SharEntry | Girişler listesinden kaldırılacak giriş. |

### Geri dönüş değeri

Paylaşım girişi örneği.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentNullException | *entry* boş. |

### Örnekler

Sonuncusu dışındaki tüm girişleri şu şekilde kaldırabilirsiniz:

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### Ayrıca bakınız

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* ad alanı [Aspose.Zip.Shar](../../shararchive/)
* toplantı [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Girişi index. ile girişler listesinden kaldırır.

```csharp
public SharArchive DeleteEntry(int entryIndex)
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
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### Ayrıca bakınız

* class [SharArchive](../)
* ad alanı [Aspose.Zip.Shar](../../shararchive/)
* toplantı [Aspose.Zip](../../../)


