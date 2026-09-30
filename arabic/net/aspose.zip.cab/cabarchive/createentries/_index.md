---
title: "CabArchive.CreateEntries"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة CabArchive. تضيف إلى الأرشيف جميع الملفات بشكل متكرر من الدليل المحدد"
type: docs
weight: 30
url: /ar/net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

تضيف إلى الأرشيف جميع الملفات، بشكل متكرر، من الدليل المحدد.

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| directory | DirectoryInfo | الدليل للضغط. |
| includeRootDirectory | Boolean | يشير إلى ما إذا كان يجب تضمين اسم الدليل الجذر في مسارات الإدخالات. |

### قيمة الإرجاع

الكائن الحالي لـ [`CabArchive`](../).

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *directory* فارغ. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| DirectoryNotFoundException | لا يمكن العثور على *directory*. |
| SecurityException | المستدعي لا يمتلك الإذن المطلوب للوصول إلى *directory* أو محتواه. |
| UnauthorizedAccessException | تم رفض الوصول إلى *directory* أو أحد ملفاته. |
| IOException | حدث خطأ I/O أثناء الوصول إلى *directory*. |
| PathTooLongException | يتجاوز مسار الإدخال المُولد الحد الأقصى للطول المحدد من النظام. |
| InvalidOperationException | الأرشيف مُعد للاستخراج ولا يمكنه إضافة إدخالات. |

## أمثلة

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### انظر أيضًا

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

يضيف إلى الأرشيف جميع الملفات بشكل متكرر من مسار الدليل المحدد.

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceDirectory | String | مسار الدليل للضغط. |
| includeRootDirectory | Boolean | يشير إلى ما إذا كان يجب تضمين اسم الدليل الجذر في مسارات الإدخالات. |

### قيمة الإرجاع

الكائن الحالي لـ [`CabArchive`](../).

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| ArgumentNullException | *sourceDirectory* فارغ. |
| DirectoryNotFoundException | *sourceDirectory* غير موجود. |
| SecurityException | المستدعي لا يمتلك الإذن المطلوب للوصول إلى *sourceDirectory*. |
| UnauthorizedAccessException | تم رفض الوصول إلى *sourceDirectory*. |
| PathTooLongException | الـ *sourceDirectory* المحدد يتجاوز الحد الأقصى للطول المحدد من النظام. |
| ArgumentException | *sourceDirectory* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| IOException | حدث خطأ I/O أثناء الوصول إلى *sourceDirectory*. |
| InvalidOperationException | الأرشيف مُعد للاستخراج ولا يمكنه إضافة إدخالات. |

## أمثلة

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### انظر أيضًا

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


