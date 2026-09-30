---
title: "IsoArchive.Save"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة IsoArchive. تحفظ صورة ISO في المسار المحدد."
type: docs
weight: 70
url: /ar/net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

يحفظ صورة ISO إلى المسار المحدد.

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار الذي سيتم حفظ صورة ISO فيه. |
| saveOptions | IsoSaveOptions | خيارات لحفظ أرشيف ISO. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | يُرمى عندما لا يكون الأرشيف في وضع التحرير. |
| ArgumentNullException | يُرمى عندما يكون *path* فارغًا. |
| DirectoryNotFoundException | يُرمى عندما يكون المسار المحدد غير صالح، مثل كونه على قرص غير مرتبط. |
| IOException | يُرمى عندما يكون الملف مفتوحًا بالفعل. |
| UnauthorizedAccessException | يُرمى عندما يُرفض الوصول إلى ملف *path*. |
| PathTooLongException | يُرمى عندما يتجاوز *path* المحدد الحد الأقصى للطول المحدد من النظام. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## أمثلة

المثال التالي يوضح كيفية حفظ أرشيف ISO إلى ملف:

```csharp
// إنشاء أرشيف ISO فارغ جديد
using(IsoArchive isoArchive = new IsoArchive())
{
    // إضافة ملفات إلى أرشيف ISO
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // حفظ أرشيف ISO إلى ملف
    isoArchive.Save("new_archive.iso");
}
```

### انظر أيضًا

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

يحفظ صورة ISO إلى الدفق المحدد.

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تيار | تيار | الدفق الذي سيتم حفظ صورة ISO فيه. |
| saveOptions | IsoSaveOptions | خيارات لحفظ أرشيف ISO. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | يُرمى عندما لا يكون الأرشيف في وضع التحرير. |
| ArgumentNullException | يُرمى عندما يكون *stream* فارغًا. |
| ArgumentException | يتم إلقاء الاستثناء عندما لا يكون *stream* قابلًا للكتابة. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| IOException | حدث خطأ في الإدخال/الإخراج. |

## أمثلة

المثال التالي يوضح كيفية حفظ أرشيف ISO إلى تدفق الذاكرة:

```csharp

 // إنشاء أرشيف ISO فارغ جديد
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // إضافة ملفات إلى أرشيف ISO
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // احفظ أرشيف ISO إلى تدفق الذاكرة
     isoArchive.Save(memoryStream);
 }
```

### انظر أيضًا

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


