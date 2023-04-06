---
title: Archive.DeleteEntry
second_title: Aspose.ZIP لمرجع .NET API
description: Archive طريقة. يزيل التكرار الأول لإدخال محدد من قائمة الإدخالات.
type: docs
weight: 60
url: /ar/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

يزيل التكرار الأول لإدخال محدد من قائمة الإدخالات.

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| entry | ArchiveEntry | الإدخال المطلوب إزالته من قائمة الإدخالات. |

### قيمة الإرجاع

الأرشيف مع الإدخال محذوف.

### أمثلة

إليك كيفية إزالة جميع الإدخالات باستثناء المدخل الأخير:

```csharp
using (var archive = new Archive("archive.zip"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save("last_entry.zip");
}
```

### أنظر أيضا

* class [ArchiveEntry](../../archiveentry/)
* class [Archive](../)
* مساحة الاسم [Aspose.Zip](../../archive/)
* المجسم [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

يحذف الإدخال من قائمة الإدخالات بالفهرس.

```csharp
public Archive DeleteEntry(int entryIndex)
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
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### أنظر أيضا

* class [Archive](../)
* مساحة الاسم [Aspose.Zip](../../archive/)
* المجسم [Aspose.Zip](../../../)


