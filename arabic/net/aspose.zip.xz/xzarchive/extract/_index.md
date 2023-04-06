---
title: XzArchive.Extract
second_title: Aspose.ZIP لمرجع .NET API
description: XzArchive طريقة. استخراج أرشيف xz إلى تيار .
type: docs
weight: 30
url: /ar/net/aspose.zip.xz/xzarchive/extract/
---
## Extract(Stream) {#extract_2}

استخراج أرشيف xz إلى تيار .

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

### أمثلة

```csharp
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new XzArchive(xzFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### أنظر أيضا

* class [XzArchive](../)
* مساحة الاسم [Aspose.Zip.Xz](../../xzarchive/)
* المجسم [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

استخراج أرشيف xz إلى ملف.

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
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### أنظر أيضا

* class [XzArchive](../)
* مساحة الاسم [Aspose.Zip.Xz](../../xzarchive/)
* المجسم [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

استخراج أرشيف xz إلى ملف حسب المسار.

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
using (FileStream xzFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new XzArchive(xzFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### أنظر أيضا

* class [XzArchive](../)
* مساحة الاسم [Aspose.Zip.Xz](../../xzarchive/)
* المجسم [Aspose.Zip](../../../)


