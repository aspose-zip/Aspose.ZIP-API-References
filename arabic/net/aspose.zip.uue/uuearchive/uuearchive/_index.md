---
title: "UueArchive.UueArchive"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "منشئ UueArchive. يهيئ نسخة جديدة من فئة UueArchive مُعدة للترميز"
type: docs
weight: 10
url: /ar/net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

يُهيئ نسخة جديدة من الفئة [`UueArchive`](../) المُعدة للترميز.

```csharp
public UueArchive()
```

## أمثلة

المثال التالي يوضح كيفية ترميز ملف باستخدام uuencode.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### انظر أيضًا

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

يُهيئ نسخة جديدة من الفئة [`UueArchive`](../) المُعدة للفك.

```csharp
public UueArchive(Stream sourceStream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | تيار | مصدر الأرشيف. |

## ملاحظات

هذا المنشئ لا يقوم بالفك. راجع طريقة [`Open`](../open/) لفك الضغط.

## أمثلة

افتح أرشيفًا من دفق واستخرجه إلى `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### انظر أيضًا

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

يُهيئ نسخة جديدة من الفئة [`UueArchive`](../).

```csharp
public UueArchive(string path)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى ملف الأرشيف. |

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
| FileNotFoundException | الملف غير موجود. |
| IOException | الملف مفتوح بالفعل. |

## ملاحظات

هذا المنشئ لا يقوم بفك الضغط. راجع طريقة [`Open`](../open/) لفك الضغط.

## أمثلة

افتح أرشيفًا من ملف عن طريق المسار وفكّ تشفيره إلى `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### انظر أيضًا

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


