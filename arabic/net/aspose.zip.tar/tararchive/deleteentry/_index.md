---
title: TarArchive.DeleteEntry
second_title: Aspose.ZIP لمرجع .NET API
description: TarArchive طريقة. يزيل التكرار الأول لإدخال محدد من قائمة الإدخالات.
type: docs
weight: 90
url: /ar/net/aspose.zip.tar/tararchive/deleteentry/
---
## DeleteEntry(TarEntry) {#deleteentry}

يزيل التكرار الأول لإدخال محدد من قائمة الإدخالات.

```csharp
public TarArchive DeleteEntry(TarEntry entry)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| entry | TarEntry | الإدخال المطلوب إزالته من قائمة الإدخالات. |

### قيمة الإرجاع

الأرشيف مع الإدخال محذوف.

### أمثلة

إليك كيفية إزالة جميع الإدخالات باستثناء المدخل الأخير:

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputTarFile);
}
```

### أنظر أيضا

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* مساحة الاسم [Aspose.Zip.Tar](../../tararchive/)
* المجسم [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

يحذف الإدخال من قائمة الإدخالات بالفهرس.

```csharp
public TarArchive DeleteEntry(int entryIndex)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| entryIndex | Int32 | الفهرس الصفري للإدخال المراد إزالته. |

### قيمة الإرجاع

الأرشيف مع الإدخال محذوف.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* أقل من 0. أو-*entryIndex* يساوي أو أكبر من`إدخالات` عدد. |

### أمثلة

```csharp
using (var archive = new TarArchive("two_files.tar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.tar");
}
```

### أنظر أيضا

* class [TarArchive](../)
* مساحة الاسم [Aspose.Zip.Tar](../../tararchive/)
* المجسم [Aspose.Zip](../../../)


