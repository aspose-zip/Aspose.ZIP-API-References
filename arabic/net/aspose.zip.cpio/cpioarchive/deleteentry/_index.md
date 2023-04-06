---
title: CpioArchive.DeleteEntry
second_title: Aspose.ZIP لمرجع .NET API
description: CpioArchive طريقة. يزيل التكرار الأول لإدخال محدد من قائمة الإدخالات.
type: docs
weight: 50
url: /ar/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

يزيل التكرار الأول لإدخال محدد من قائمة الإدخالات.

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| entry | CpioEntry | الإدخال المطلوب إزالته من قائمة الإدخالات. |

### قيمة الإرجاع

مثيل إدخال Cpio.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *entry* باطل. |

### أمثلة

إليك كيفية إزالة جميع الإدخالات باستثناء المدخل الأخير:

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### أنظر أيضا

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* مساحة الاسم [Aspose.Zip.Cpio](../../cpioarchive/)
* المجسم [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

يحذف الإدخال من قائمة الإدخالات بالفهرس.

```csharp
public CpioArchive DeleteEntry(int entryIndex)
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
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### أنظر أيضا

* class [CpioArchive](../)
* مساحة الاسم [Aspose.Zip.Cpio](../../cpioarchive/)
* المجسم [Aspose.Zip](../../../)


