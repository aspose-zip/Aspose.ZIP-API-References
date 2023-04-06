---
title: Archive.CreateEntries
second_title: Aspose.ZIP لمرجع .NET API
description: Archive طريقة. يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المعطى.
type: docs
weight: 40
url: /ar/net/aspose.zip/archive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المعطى.

```csharp
public Archive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| directory | DirectoryInfo | دليل لضغط. |
| includeRootDirectory | Boolean | يشير إلى ما إذا كان سيتم تضمين الدليل الجذر نفسه أم لا. |

### قيمة الإرجاع

يتكون الأرشيف مع الإدخالات.

### استثناءات

| استثناء | حالة |
| --- | --- |
| DirectoryNotFoundException | الطريق إلى*directory* غير صالح ، مثل وجوده على محرك أقراص غير معين. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول*directory*. |

### أمثلة

```csharp
using (Archive archive = new Archive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.zip");
}
```

### أنظر أيضا

* class [Archive](../)
* مساحة الاسم [Aspose.Zip](../../archive/)
* المجسم [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المعطى.

```csharp
public Archive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| sourceDirectory | String | دليل لضغط. |
| includeRootDirectory | Boolean | يشير إلى ما إذا كان سيتم تضمين الدليل الجذر نفسه أم لا. |

### قيمة الإرجاع

يتكون الأرشيف مع الإدخالات.

### أمثلة

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.zip");
}
```

### أنظر أيضا

* class [Archive](../)
* مساحة الاسم [Aspose.Zip](../../archive/)
* المجسم [Aspose.Zip](../../../)


