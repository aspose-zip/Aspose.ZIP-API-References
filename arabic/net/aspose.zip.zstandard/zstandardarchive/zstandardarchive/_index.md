---
title: "ZstandardArchive.ZstandardArchive"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "منشئ ZstandardArchive. يهيئ نسخة جديدة من فئة ZstandardArchive مُعدة للضغط"
type: docs
weight: 10
url: /ar/net/aspose.zip.zstandard/zstandardarchive/zstandardarchive/
---
## ZstandardArchive() {#constructor}

يهيئ نسخة جديدة من فئة [`ZstandardArchive`](../) مُعدة للضغط.

```csharp
public ZstandardArchive()
```

## أمثلة

المثال التالي يوضح كيفية ضغط ملف.

```csharp
using (ZstandardArchive archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### انظر أيضًا

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(Stream, ZstandardLoadOptions) {#constructor_1}

يهيئ نسخة جديدة من فئة [`ZstandardArchive`](../) مُعدة لفك الضغط.

```csharp
public ZstandardArchive(Stream sourceStream, ZstandardLoadOptions options = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | تيار | مصدر الأرشيف. |
| خيارات | ZstandardLoadOptions | الخيارات لتحميل الأرشيف بها. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | يُرمى إذا تم التخلص من تدفق المصدر. |
| EndOfStreamException | يُرمى عندما يتم الوصول إلى نهاية التدفق بشكل غير متوقع. |
| IOException | حدث خطأ في الإدخال/الإخراج. |
| InvalidDataException | يتم إلقاؤه عندما تكون البيانات غير صالحة أو تالفة. |

## ملاحظات

هذا المنشئ لا يقوم بفك الضغط. راجع طريقة [`Open`](../open/) لفك الضغط.

## أمثلة

افتح أرشيفًا من دفق واستخرجه إلى `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new ZstandardArchive(File.OpenRead("archive.zst")))
  archive.Open().CopyTo(ms);
```

### انظر أيضًا

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(string, ZstandardLoadOptions) {#constructor_2}

يهيئ نسخة جديدة من فئة [`ZstandardArchive`](../).

```csharp
public ZstandardArchive(string path, ZstandardLoadOptions options = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى ملف الأرشيف. |
| خيارات | ZstandardLoadOptions | الخيارات لتحميل الأرشيف بها. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *path* فارغ. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول. |
| ArgumentException | المسار *path* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *path*. |
| PathTooLongException | الـ *path* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *path* يحتوي على نقطتين (:) في وسط السلسلة. |
| DirectoryNotFoundException | المسار المحدد غير صالح، مثل كونه على قرص غير مرتبط. |
| EndOfStreamException | يُرمى عندما يتم الوصول إلى نهاية التدفق بشكل غير متوقع. |
| FileNotFoundException | الملف غير موجود. |
| IOException | الملف مفتوح بالفعل. |
| InvalidDataException | يتم إلقاؤه عندما تكون البيانات غير صالحة أو تالفة. |

## ملاحظات

هذا المنشئ لا يقوم بفك الضغط. راجع طريقة [`Open`](../open/) لفك الضغط.

## أمثلة

افتح أرشيفًا من ملف عبر المسار واستخرجه إلى `MemoryStream`

```csharp
var ms = new MemoryStream();
using (ZstandardArchive archive = new ZstandardArchive("archive.zst"))
  archive.Open().CopyTo(ms);
```

### انظر أيضًا

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


