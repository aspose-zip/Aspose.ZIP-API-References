---
title: SharArchive.DeleteEntry
second_title: Aspose.ZIP لمرجع .NET API
description: SharArchive طريقة. يزيل التكرار الأول لإدخال محدد من قائمة الإدخالات.
type: docs
weight: 50
url: /ar/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

يزيل التكرار الأول لإدخال محدد من قائمة الإدخالات.

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| entry | SharEntry | الإدخال المطلوب إزالته من قائمة الإدخالات. |

### قيمة الإرجاع

مثيل دخول المشاركة.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *entry* باطل. |

### أمثلة

إليك كيفية إزالة جميع الإدخالات باستثناء المدخل الأخير:

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### أنظر أيضا

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* مساحة الاسم [Aspose.Zip.Shar](../../shararchive/)
* المجسم [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

يحذف الإدخال من قائمة الإدخالات بالفهرس.

```csharp
public SharArchive DeleteEntry(int entryIndex)
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
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### أنظر أيضا

* class [SharArchive](../)
* مساحة الاسم [Aspose.Zip.Shar](../../shararchive/)
* المجسم [Aspose.Zip](../../../)


