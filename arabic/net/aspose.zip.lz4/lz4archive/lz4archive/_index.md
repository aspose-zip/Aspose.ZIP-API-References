---
title: "Lz4Archive.Lz4Archive"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "منشئ Lz4Archive. يهيئ نسخة جديدة من فئة Lz4Archive مُجهزة للفك."
type: docs
weight: 10
url: /ar/net/aspose.zip.lz4/lz4archive/lz4archive/
---
## Lz4Archive(Stream, Lz4LoadOptions) {#constructor_1}

يهيئ نسخة جديدة من الفئة [`Lz4Archive`](../) المُجهزة للفك.

```csharp
public Lz4Archive(Stream sourceStream, Lz4LoadOptions loadOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | تيار | مصدر الأرشيف. |
| loadOptions | Lz4LoadOptions | الخيارات لتحميل الأرشيف بها. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | لا يمكن القراءة من *sourceStream* |
| ArgumentNullException | *sourceStream* هو null. |
| EndOfStreamException | *sourceStream* قصير جدًا. |
| InvalidDataException | *sourceStream* يحتوي على توقيع غير صحيح. |
| ObjectDisposedException | يُرمى إذا تم التخلص من تدفق المصدر. |
| IOException | حدث خطأ في الإدخال/الإخراج. |

## ملاحظات

هذا المنشئ لا يقوم بفك الضغط. راجع طريقة [`Open`](../open/) لفك الضغط.

## أمثلة

افتح أرشيفًا من دفق واستخرجه إلى `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive(File.OpenRead("archive.lz4")))
  archive.Open().CopyTo(ms);
```

### انظر أيضًا

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(string, Lz4LoadOptions) {#constructor_2}

يهيئ نسخة جديدة من الفئة [`Lz4Archive`](../).

```csharp
public Lz4Archive(string path, Lz4LoadOptions loadOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى ملف الأرشيف. |
| loadOptions | Lz4LoadOptions | الخيارات لتحميل الأرشيف بها. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *path* فارغ. |
| SecurityException | المستدعي لا يمتلك الإذن المطلوب للوصول |
| ArgumentException | المسار *path* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *path*. |
| PathTooLongException | الـ *path* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *path* يحتوي على نقطتين (:) في وسط السلسلة. |
| EndOfStreamException | الملف قصير جدًا. |
| InvalidDataException | البيانات في الملف لها توقيع غير صحيح. |
| DirectoryNotFoundException | المسار المحدد غير صالح، مثل كونه على قرص غير مرتبط. |
| FileNotFoundException | الملف غير موجود. |
| IOException | الملف مفتوح بالفعل. |

## ملاحظات

هذا المنشئ لا يقوم بفك الضغط. راجع طريقة [`Open`](../open/) لفك الضغط.

## أمثلة

افتح أرشيفًا من ملف عبر المسار واستخرجه إلى `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive("archive.lz4"))
  archive.Open().CopyTo(ms);
```

### انظر أيضًا

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(Lz4ArchiveSetting) {#constructor}

يهيئ نسخة جديدة من الفئة [`Lz4Archive`](../) المُجهزة للضغط.

```csharp
public Lz4Archive(Lz4ArchiveSetting settings = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الإعدادات | Lz4ArchiveSetting | إعداد الأرشيف المركب. |

### انظر أيضًا

* class [Lz4ArchiveSetting](../../lz4archivesetting/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


