---
title: Archive.DeleteEntry
second_title: Aspose.ZIP for .NET API Referansı
description: Archive yöntem. Belirli bir girişin ilk örneğini girişler listesinden kaldırır.
type: docs
weight: 60
url: /tr/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

Belirli bir girişin ilk örneğini girişler listesinden kaldırır.

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| entry | ArchiveEntry | Girişler listesinden kaldırılacak giriş. |

### Geri dönüş değeri

Girişin silindiği arşiv.

### Örnekler

Sonuncusu dışındaki tüm girişleri şu şekilde kaldırabilirsiniz:

```csharp
using (var archive = new Archive("archive.zip"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save("last_entry.zip");
}
```

### Ayrıca bakınız

* class [ArchiveEntry](../../archiveentry/)
* class [Archive](../)
* ad alanı [Aspose.Zip](../../archive/)
* toplantı [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Girişi index. ile girişler listesinden kaldırır.

```csharp
public Archive DeleteEntry(int entryIndex)
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
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### Ayrıca bakınız

* class [Archive](../)
* ad alanı [Aspose.Zip](../../archive/)
* toplantı [Aspose.Zip](../../../)


