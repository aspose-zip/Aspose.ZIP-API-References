---
title: "ArjArchive.ArjArchive"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "منشئ ArjArchive. يهيئ نسخة جديدة من فئة ArjArchive ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف."
type: docs
weight: 10
url: /ar/net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream, ArjLoadOptions) {#constructor}

يهيئ نسخة جديدة من الفئة [`ArjArchive`](../) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

```csharp
public ArjArchive(Stream extractionSource, ArjLoadOptions loadOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| extractionSource | تيار | مصدر الأرشيف. |
| loadOptions | ArjLoadOptions | خيارات لتحميل الأرشيف الموجود. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *extractionSource* فارغ. |
| ArgumentException | &gt;*extractionSource* لا يدعم التمرير. |
| InvalidDataException | توقيع غير صحيح للأرشيف. - أو - الملف ليس أرشيف ARJ. |
| EndOfStreamException | يتم رمي الاستثناء عندما يتم الوصول إلى نهاية الدفق قبل قراءة جميع بايتات الرأس أو بايتات الاسم. |
| NotSupportedException | الأرشيف مشوّه. |

## ملاحظات

هذا المُنشئ لا يفك ضغط أي إدخال. راجع طريقة [`Extract`](../../arjentryplain/extract/) لفك الضغط.

### انظر أيضًا

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string, ArjLoadOptions) {#constructor_1}

يهيئ نسخة جديدة من الفئة [`ArjArchive`](../) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

```csharp
public ArjArchive(string path, ArjLoadOptions loadOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى ملف الأرشيف. |
| loadOptions | ArjLoadOptions | خيارات لتحميل الأرشيف الموجود. |

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
| EndOfStreamException | يتم رمي الاستثناء عندما يتم الوصول إلى نهاية الدفق قبل قراءة جميع بايتات الرأس أو بايتات الاسم. |
| InvalidDataException | رقم السحر الخاص بـ ARJ غير صالح أو حجم الرأس خارج النطاق. |

## ملاحظات

هذا المُنشئ لا يفك أي إدخال. راجع طريقة [`Extract`](../../arjentryplain/extract/) لفك الضغط.

## أمثلة

المثال التالي يوضح كيفية استخراج جميع الإدخالات إلى مجلد.

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### انظر أيضًا

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


