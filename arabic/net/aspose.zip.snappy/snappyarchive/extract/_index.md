---
title: SnappyArchive.Extract
second_title: Aspose.ZIP لمرجع .NET API
description: SnappyArchive طريقة. استخراج أرشيف سريع إلى تيار .
type: docs
weight: 30
url: /ar/net/aspose.zip.snappy/snappyarchive/extract/
---
## Extract(Stream) {#extract_2}

استخراج أرشيف سريع إلى تيار .

```csharp
public void Extract(Stream destination)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| destination | Stream | دفق لتخزين البيانات غير المضغوطة. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| InvalidOperationException | لم يتم قراءة رؤوس الأرشيف ومعلومات الخدمة. |
| InvalidDataException | خطأ في البيانات في العنوان أو المجموع الاختباري. |
| ArgumentNullException | تيار الوجهة فارغ. |
| ArgumentException | دفق الوجهة لا يدعم الكتابة. |

### أمثلة

```csharp
using (FileStream sourceSnappyFile = File.Open(sourceFileName, FileMode.Open))
{
   using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
   {
       using (var archive = new SnappyArchive(sourceSnappyFile))
       {
           archive.Extract(extractedFile);
       }
   }
}
```

### أنظر أيضا

* class [SnappyArchive](../)
* مساحة الاسم [Aspose.Zip.Snappy](../../snappyarchive/)
* المجسم [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

استخراج أرشيف سريع إلى ملف.

```csharp
public void Extract(FileInfo fileInfo)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo لتخزين البيانات التي تم فك ضغطها. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| InvalidOperationException | لم يتم قراءة رؤوس الأرشيف ومعلومات الخدمة. |
| SecurityException | المتصل ليس لديه الإذن المطلوب لفتح*fileInfo*. |
| ArgumentException | مسار الملف فارغ أو يحتوي على مسافات بيضاء فقط. |
| FileNotFoundException | لم يتم العثور على الملف. |
| UnauthorizedAccessException | مسار الملف للقراءة فقط أو هو دليل. |
| ArgumentNullException | *fileInfo* باطل. |
| DirectoryNotFoundException | المسار المحدد غير صالح ، مثل وجوده على محرك أقراص غير معين. |
| IOException | الملف مفتوح بالفعل. |

### أمثلة

```csharp
using (FileStream snappyFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new SnappyArchive(snappyFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### أنظر أيضا

* class [SnappyArchive](../)
* مساحة الاسم [Aspose.Zip.Snappy](../../snappyarchive/)
* المجسم [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

استخراج أرشيف سريع إلى ملف عن طريق المسار.

```csharp
public FileInfo Extract(string path)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | مسار الملف الذي سيخزن البيانات غير المضغوطة. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| InvalidOperationException | لم يتم قراءة رؤوس الأرشيف ومعلومات الخدمة. |
| ArgumentNullException | *path* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول. |
| ArgumentException | ال*path* فارغ أو يحتوي على مسافات بيضاء فقط أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | الوصول إلى الملف*path* مرفوض. |
| PathTooLongException | المحدد*path*أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ، ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | ملف في*path* يحتوي على نقطتين (:) في منتصف السلسلة. |

### أمثلة

```csharp
using (FileStream snappyFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new SnappyArchive(snappyFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### أنظر أيضا

* class [SnappyArchive](../)
* مساحة الاسم [Aspose.Zip.Snappy](../../snappyarchive/)
* المجسم [Aspose.Zip](../../../)


