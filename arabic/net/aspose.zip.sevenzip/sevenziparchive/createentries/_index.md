---
title: SevenZipArchive.CreateEntries
second_title: Aspose.ZIP لمرجع .NET API
description: SevenZipArchive طريقة. يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المعطى.
type: docs
weight: 40
url: /ar/net/aspose.zip.sevenzip/sevenziparchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المعطى.

```csharp
public SevenZipArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
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
using (SevenZipArchive archive = new SevenZipArchive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.7z");
}
```

### أنظر أيضا

* class [SevenZipArchive](../)
* مساحة الاسم [Aspose.Zip.SevenZip](../../sevenziparchive/)
* المجسم [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

يضيف إلى الأرشيف جميع الملفات والمجلدات بشكل متكرر في الدليل المعطى.

```csharp
public SevenZipArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| sourceDirectory | String | دليل لضغط. |
| includeRootDirectory | Boolean | يشير إلى ما إذا كان سيتم تضمين الدليل الجذر نفسه أم لا. |

### قيمة الإرجاع

يتكون الأرشيف مع الإدخالات.

### أمثلة

يؤلف أرشيف 7z بضغط LZMA2.

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.7z");
}
```

### أنظر أيضا

* class [SevenZipArchive](../)
* مساحة الاسم [Aspose.Zip.SevenZip](../../sevenziparchive/)
* المجسم [Aspose.Zip](../../../)


