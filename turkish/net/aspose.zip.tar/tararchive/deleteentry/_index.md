---
title: TarArchive.DeleteEntry
second_title: Aspose.ZIP for .NET API Referansı
description: TarArchive yöntem. Belirli bir girişin ilk örneğini girişler listesinden kaldırır.
type: docs
weight: 90
url: /tr/net/aspose.zip.tar/tararchive/deleteentry/
---
## DeleteEntry(TarEntry) {#deleteentry}

Belirli bir girişin ilk örneğini girişler listesinden kaldırır.

```csharp
public TarArchive DeleteEntry(TarEntry entry)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| entry | TarEntry | Girişler listesinden kaldırılacak giriş. |

### Geri dönüş değeri

Girişin silindiği arşiv.

### Örnekler

Sonuncusu dışındaki tüm girişleri şu şekilde kaldırabilirsiniz:

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputTarFile);
}
```

### Ayrıca bakınız

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Girişi index. ile girişler listesinden kaldırır.

```csharp
public TarArchive DeleteEntry(int entryIndex)
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
using (var archive = new TarArchive("two_files.tar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.tar");
}
```

### Ayrıca bakınız

* class [TarArchive](../)
* ad alanı [Aspose.Zip.Tar](../../tararchive/)
* toplantı [Aspose.Zip](../../../)


