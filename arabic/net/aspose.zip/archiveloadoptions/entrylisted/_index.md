---
title: ArchiveLoadOptions.EntryListed
second_title: Aspose.ZIP لمرجع .NET API
description: ArchiveLoadOptions ملكية. الحصول على المفوض الذي تم استدعاؤه أو تعيينه عند إدخال مُدرج في جدول المحتويات.
type: docs
weight: 50
url: /ar/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

الحصول على المفوض الذي تم استدعاؤه أو تعيينه عند إدخال مُدرج في جدول المحتويات.

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

### أمثلة

```csharp
Archive archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### أنظر أيضا

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* مساحة الاسم [Aspose.Zip](../../archiveloadoptions/)
* المجسم [Aspose.Zip](../../../)


