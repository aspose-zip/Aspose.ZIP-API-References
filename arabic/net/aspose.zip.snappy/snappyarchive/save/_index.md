---
title: SnappyArchive.Save
second_title: Aspose.ZIP لمرجع .NET API
description: SnappyArchive طريقة. يحفظ أرشيفًا سريعًا في الدفق المقدم.
type: docs
weight: 40
url: /ar/net/aspose.zip.snappy/snappyarchive/save/
---
## Save(Stream) {#save_1}

يحفظ أرشيفًا سريعًا في الدفق المقدم.

```csharp
public void Save(Stream output)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| output | Stream | تيار الوجهة. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentException | *output* لا يدعم السعي. |
| ArgumentNullException | *output* باطل. |

### ملاحظات

*output* يجب أن يكون قابلاً للبحث.

### أمثلة

```csharp
using (FileStream snappyFile = File.Open("archive.snappy", FileMode.Create))
{
    using (var archive = new SnappyArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(snappyFile);
     }
}
```

### أنظر أيضا

* class [SnappyArchive](../)
* مساحة الاسم [Aspose.Zip.Snappy](../../snappyarchive/)
* المجسم [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

يحفظ الأرشيف السريع في ملف الوجهة المقدم.

```csharp
public void Save(FileInfo destination)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| destination | FileInfo | FileInfo الذي سيتم فتحه كتدفق الوجهة. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| SecurityException | المتصل ليس لديه الإذن المطلوب لفتح*destination*. |
| ArgumentException | مسار الملف فارغ أو يحتوي على مسافات بيضاء فقط. |
| FileNotFoundException | لم يتم العثور على الملف. |
| UnauthorizedAccessException | مسار الملف للقراءة فقط أو هو دليل. |
| ArgumentNullException | *destination* باطل. |
| DirectoryNotFoundException | المسار المحدد غير صالح ، مثل وجوده على محرك أقراص غير معين. |
| IOException | الملف مفتوح بالفعل. |

### أمثلة

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.snappy"));
}
```

### أنظر أيضا

* class [SnappyArchive](../)
* مساحة الاسم [Aspose.Zip.Snappy](../../snappyarchive/)
* المجسم [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

يحفظ الأرشيف السريع في ملف الوجهة المقدم.

```csharp
public void Save(string destinationFileName)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| destinationFileName | String | مسار الأرشيف المراد إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود ، فسيتم استبداله. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *destinationFileName* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول. |
| ArgumentException | ال*destinationFileName* فارغ أو يحتوي على مسافات بيضاء فقط أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | الوصول إلى الملف*destinationFileName* مرفوض. |
| PathTooLongException | المحدد*destinationFileName*أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ، ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | ملف في*destinationFileName* يحتوي على نقطتين (:) في منتصف السلسلة. |

### أمثلة

```csharp
using (var archive = new SnappyArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.snappy");
}
```

### أنظر أيضا

* class [SnappyArchive](../)
* مساحة الاسم [Aspose.Zip.Snappy](../../snappyarchive/)
* المجسم [Aspose.Zip](../../../)


