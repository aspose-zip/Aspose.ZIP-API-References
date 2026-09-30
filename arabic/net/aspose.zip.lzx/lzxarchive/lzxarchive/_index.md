---
title: "LzxArchive.LzxArchive"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "منشئ LzxArchive. يهيء مثيلاً جديداً لفئة LzxArchive ويُنشئ قائمة إدخالات يمكن استخراجها من الأرشيف"
type: docs
weight: 10
url: /ar/net/aspose.zip.lzx/lzxarchive/lzxarchive/
---
## LzxArchive(Stream, LzxLoadOptions) {#constructor}

يهيء مثيلاً جديداً لفئة [`LzxArchive`](../) ويُنشئ قائمة إدخالات يمكن استخراجها من الأرشيف.

```csharp
public LzxArchive(Stream extractionSource, LzxLoadOptions loadOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| extractionSource | تيار | مصدر الأرشيف. |
| loadOptions | LzxLoadOptions | خيارات لتحميل الأرشيف الموجود. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *extractionSource* فارغ. |
| ArgumentException | *extractionSource* لا يدعم السعي. |
| InvalidDataException | توقيع غير صحيح للأرشيف. - أو - الملف ليس أرشيف LZX. |
| NotImplementedException | أرشيف Lzx يحتوي على إدخالات مدمجة. |
| EndOfStreamException | تدفق *extractionSource* قصير جداً. |
| ObjectDisposedException | يُرمى إذا تم إغلاق التدفق. |
| IOException | حدث خطأ في الإدخال/الإخراج. |

## ملاحظات

هذا المنشئ لا يفك ضغط أي إدخال. راجع طريقة [`Extract`](../../lzxarchiveentry/extract/) لفك الضغط.

### انظر أيضًا

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)

---

## LzxArchive(string, LzxLoadOptions) {#constructor_1}

يهيء مثيلاً جديداً لفئة [`LzxArchive`](../) ويُنشئ قائمة إدخالات يمكن استخراجها من الأرشيف.

```csharp
public LzxArchive(string path, LzxLoadOptions loadOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار المؤهل بالكامل أو المسار النسبي إلى ملف الأرشيف. |
| loadOptions | LzxLoadOptions | خيارات لتحميل الأرشيف الموجود. |

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
| NotImplementedException | أرشيف Lzx يحتوي على إدخالات مدمجة. |
| EndOfStreamException | الملف قصير جدًا. |
| ObjectDisposedException | يُرمى إذا تم إغلاق التدفق. |

## ملاحظات

هذا المنشئ لا يفك ضغط أي إدخال. راجع طريقة [`Extract`](../../lzxarchiveentry/extract/) لفك الضغط.

## أمثلة

المثال التالي يستخرج أرشيفًا، ثم يفك ضغط العنصر الأول إلى `MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (LzxArchive archive = new LzxArchive("sample.lzx"))
{
    archive.Entries[0].Extract(extracted);
}
```

### انظر أيضًا

* class [LzxLoadOptions](../../lzxloadoptions/)
* class [LzxArchive](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchive/)
* assembly [Aspose.Zip](../../../)


