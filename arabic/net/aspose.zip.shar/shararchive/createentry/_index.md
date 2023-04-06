---
title: SharArchive.CreateEntry
second_title: Aspose.ZIP لمرجع .NET API
description: SharArchive طريقة. إنشاء إدخال واحد داخل الأرشيف.
type: docs
weight: 40
url: /ar/net/aspose.zip.shar/shararchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public SharEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| name | String | اسم الإدخال. |
| fileInfo | FileInfo | البيانات الوصفية للملف أو المجلد المراد ضغطه. |
| openImmediately | Boolean | صحيح إذا فتحت الملف على الفور ، وإلا فافتح الملف عند حفظ الأرشيف. |

### قيمة الإرجاع

مثيل دخول المشاركة.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *name* باطل. |
| ArgumentException | *name* فارغ. |
| ArgumentNullException | *fileInfo* باطل. |

### ملاحظات

إذا تم فتح الملف على الفور باستخدام*openImmediately*المعلمة يتم حظرها حتى يتم التخلص من الأرشيف.

### أمثلة

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new SharArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.shar");
}
```

### أنظر أيضا

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* مساحة الاسم [Aspose.Zip.Shar](../../shararchive/)
* المجسم [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public SharEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| name | String | اسم الإدخال. |
| sourcePath | String | مسار الملف المراد ضغطه. |
| openImmediately | Boolean | صحيح إذا فتحت الملف على الفور ، وإلا فافتح الملف عند حفظ الأرشيف. |

### قيمة الإرجاع

مثيل دخول المشاركة.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *sourcePath* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول. |
| ArgumentException | ال*sourcePath* فارغ أو يحتوي على مسافات بيضاء فقط أو يحتوي على أحرف غير صالحة. - أو - اسم الملف ، كجزء من*name*، يتجاوز 100 رمز. |
| UnauthorizedAccessException | الوصول إلى الملف*sourcePath* مرفوض. |
| PathTooLongException | المحدد*sourcePath* أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ، ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. - أو -*name* طويل جدًا بالنسبة إلى المشاركة. |
| NotSupportedException | ملف في*sourcePath* يحتوي على نقطتين (:) في منتصف السلسلة. |

### ملاحظات

تم تعيين اسم الإدخال فقط داخل*name* معامل. اسم الملف المقدم في*sourcePath* لا تؤثر المعلمة على اسم الإدخال.

إذا تم فتح الملف على الفور باستخدام*openImmediately*المعلمة يتم حظرها حتى يتم التخلص من الأرشيف.

### أمثلة

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### أنظر أيضا

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* مساحة الاسم [Aspose.Zip.Shar](../../shararchive/)
* المجسم [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public SharEntry CreateEntry(string name, Stream source)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| name | String | اسم الإدخال. |
| source | Stream | تيار الإدخال للدخول. |

### قيمة الإرجاع

مثيل دخول المشاركة.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *name* باطل. |
| ArgumentNullException | *source* باطل. |
| ArgumentException | *name* فارغ. |

### أمثلة

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.shar");
}
```

### أنظر أيضا

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* مساحة الاسم [Aspose.Zip.Shar](../../shararchive/)
* المجسم [Aspose.Zip](../../../)


