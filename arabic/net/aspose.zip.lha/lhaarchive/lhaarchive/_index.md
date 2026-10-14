---
title: "LhaArchive.LhaArchive"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "منشئ LhaArchive. يهيئ نسخة جديدة من فئة LhaArchive ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف."
type: docs
weight: 10
url: /ar/net/aspose.zip.lha/lhaarchive/lhaarchive/
---
## LhaArchive(Stream, LhaLoadOptions) {#constructor}

يهيئ نسخة جديدة من الفئة [`LhaArchive`](../) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

```csharp
public LhaArchive(Stream sourceStream, LhaLoadOptions loadOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | تيار | مصدر الأرشيف. |
| loadOptions | LhaLoadOptions | خيارات لتحميل الأرشيف الموجود. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *sourceStream* هو null |
| ArgumentException | *sourceStream* غير قابل للتمرير. |
| InvalidDataException | تم العثور على بيانات غير مناسبة. |
| EndOfStreamException | يتم إلقاؤه عندما يتم الوصول إلى نهاية الدفق قبل قراءة عدد البايتات المتوقع. |
| ObjectDisposedException | يتم رمي الاستثناء عندما يتم التخلص من الكائن. |

## ملاحظات

هذا المُنشئ لا يفك ضغط أي عنصر. راجع طريقة [`Extract`](../../lhaarchiveentry/extract/) لفك الضغط.

### انظر أيضًا

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LhaArchive(string, LhaLoadOptions) {#constructor_1}

يهيئ نسخة جديدة من الفئة [`LhaArchive`](../) ويكوّن قائمة إدخالات يمكن استخراجها من الأرشيف.

```csharp
public LhaArchive(string path, LhaLoadOptions loadOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار المؤهل بالكامل أو المسار النسبي إلى ملف الأرشيف. |
| loadOptions | LhaLoadOptions | خيارات لتحميل الأرشيف الموجود. |

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
| InvalidDataException | الملف تالف. |
| EndOfStreamException | يتم إلقاؤه عندما يتم الوصول إلى نهاية الدفق قبل قراءة عدد البايتات المتوقع. |
| ObjectDisposedException | يتم رمي الاستثناء عندما يتم التخلص من الكائن. |

## ملاحظات

هذا المُنشئ لا يفك ضغط أي عنصر. راجع طريقة [`Extract`](../../lhaarchiveentry/extract/) لفك الضغط.

## أمثلة

المثال التالي يستخرج أرشيفًا، ثم يفك ضغط العنصر الأول إلى `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LhaArchive archive = new LhaArchive("sample.lzh"))
{
    archive.Entries[0].Extract(extracted);
}
```

### انظر أيضًا

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


