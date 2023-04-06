---
title: SharArchive.CreateEntries
second_title: Aspose.ZIP لمرجع .NET API
description: SharArchive طريقة. يضيف إلى الأرشيف جميع الملفات والدلائل بشكل متكرر في الدليل المعطى.
type: docs
weight: 30
url: /ar/net/aspose.zip.shar/shararchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

يضيف إلى الأرشيف جميع الملفات والدلائل بشكل متكرر في الدليل المعطى.

```csharp
public SharArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| sourceDirectory | String | دليل لضغط. |
| includeRootDirectory | Boolean | يشير إلى ما إذا كان سيتم تضمين الدليل الجذر نفسه أم لا. |

### قيمة الإرجاع

مثيل دخول المشاركة.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *sourceDirectory* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول*sourceDirectory*. |
| ArgumentException | *sourceDirectory* يحتوي على أحرف غير صالحة مثل "أو &lt;أو&gt; أو &#x7C;. |
| PathTooLongException | المسار المحدد أو اسم الملف أو كلاهما يتجاوز الطول الأقصى المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ، ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. المسار المحدد أو اسم الملف أو كلاهما طويل جدًا. |
| IOException | *sourceDirectory* لتقف على ملف وليس دليل. |

### أمثلة

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(sharFile);
    }
}
```

### أنظر أيضا

* class [SharArchive](../)
* مساحة الاسم [Aspose.Zip.Shar](../../shararchive/)
* المجسم [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

يضيف إلى الأرشيف جميع الملفات والدلائل بشكل متكرر في الدليل المعطى.

```csharp
public SharArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| directory | DirectoryInfo | دليل لضغط. |
| includeRootDirectory | Boolean | يشير إلى ما إذا كان سيتم تضمين الدليل الجذر نفسه أم لا. |

### قيمة الإرجاع

مثيل دخول المشاركة.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *directory* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول*directory*. |
| IOException | *directory* لتقف على ملف وليس دليل. |

### أمثلة

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(sharFile);
    }
}
```

### أنظر أيضا

* class [SharArchive](../)
* مساحة الاسم [Aspose.Zip.Shar](../../shararchive/)
* المجسم [Aspose.Zip](../../../)


