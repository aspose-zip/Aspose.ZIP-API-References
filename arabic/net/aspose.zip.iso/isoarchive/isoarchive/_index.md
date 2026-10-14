---
title: "IsoArchive.IsoArchive"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "منشئ IsoArchive. يهيئ نسخة جديدة من فئة IsoArchive وينشئ أرشيف ISO فارغ لإضافة ملفات ومجلدات جديدة"
type: docs
weight: 10
url: /ar/net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

يهيئ نسخة جديدة من الفئة [`IsoArchive`](../) وينشئ أرشيف ISO فارغ لإضافة ملفات ومجلدات جديدة.

```csharp
public IsoArchive()
```

## أمثلة

المثال التالي يوضح كيفية إنشاء أرشيف ISO فارغ جديد وإضافة ملفات إليه:

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

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

يهيئ نسخة جديدة من الفئة [`IsoArchive`](../) ويُنشئ قائمة إدخالات يمكن استخراجها من الأرشيف.

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | تيار | مصدر الأرشيف. يجب أن يكون قابلًا للتمرير. |
| loadOptions | IsoLoadOptions | الخيارات لتحميل الأرشيف بها. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *sourceStream* هو null. |
| ArgumentException | *sourceStream* غير قابل للتمرير. |
| InvalidDataException | *sourceStream* ليس أرشيف ISO صالح. |
| ObjectDisposedException | يُرمى إذا تم التخلص من تدفق المصدر. |
| EndOfStreamException | يُرمى عندما يتم الوصول إلى نهاية التدفق بشكل غير متوقع. |
| IOException | حدث خطأ في الإدخال/الإخراج. |
| NotSupportedException | التدفق لا يدعم القراءة. |

## ملاحظات

هذا المنشئ لا يفك أي إدخال.

## أمثلة

المثال التالي يوضح كيفية استخراج جميع الإدخالات إلى مجلد.

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### انظر أيضًا

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

يهيئ نسخة جديدة من الفئة [`IsoArchive`](../) ويُنشئ قائمة إدخالات يمكن استخراجها من الأرشيف.

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى ملف الأرشيف. |
| loadOptions | IsoLoadOptions | الخيارات لتحميل الأرشيف بها. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *path* فارغ. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول. |
| ArgumentException | المسار *path* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *path*. |
| PathTooLongException | الـ *path* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *path* يحتوي على نقطتين (:) في وسط السلسلة. |
| FileNotFoundException | الملف غير موجود. |
| DirectoryNotFoundException | المسار المحدد غير صالح، مثل كونه على قرص غير مرتبط. |
| IOException | الملف مفتوح بالفعل. |
| EndOfStreamException | الملف قصير جدًا. |
| InvalidDataException | يتم إلقاؤه عندما تكون البيانات غير صالحة أو تالفة. |

## ملاحظات

هذا المنشئ لا يفك أي إدخال.

## أمثلة

المثال التالي يوضح كيفية استخراج جميع الإدخالات إلى مجلد.

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### انظر أيضًا

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


