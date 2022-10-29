---
title: DeleteEntry
second_title: Aspose.ZIP for .NET API Referansı
description: Belirli bir girdinin ilk oluşumunu girdiler listesinden kaldırır.
type: docs
weight: 60
url: /tr/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

Belirli bir girdinin ilk oluşumunu girdiler listesinden kaldırır.

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

* class [ArchiveEntry](../../archiveentry)
* class [Archive](../../archive)
* ad alanı [Aspose.Zip](../../archive)
* toplantı [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Girişi, dizine göre giriş listesinden kaldırır.

```csharp
public Archive DeleteEntry(int entryIndex)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| entryIndex | Int32 | Kaldırılacak girdinin sıfır tabanlı dizini. |

### Geri dönüş değeri

Girişin silindiği arşiv.

### istisnalar

| istisna | şart |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* 0.-veya-'dan küçük*entryIndex* eşittir veya daha büyüktür`Girdileri` saymak. |

### Örnekler

```csharp
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### Ayrıca bakınız

* class [Archive](../../archive)
* ad alanı [Aspose.Zip](../../archive)
* toplantı [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->