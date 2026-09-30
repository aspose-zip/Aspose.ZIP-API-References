---
title: "UueArchive.SetSource"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة UueArchive. تحدد المحتوى الذي سيتم ترميزه داخل الأرشيف"
type: docs
weight: 80
url: /ar/net/aspose.zip.uue/uuearchive/setsource/
---
## SetSource(Stream) {#setsource_1}

يضبط المحتوى الذي سيتم ترميزه داخل الأرشيف.

```csharp
public void SetSource(Stream source)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | تيار | دفق الإدخال للأرشيف. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## أمثلة

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.uue");
}
```

### انظر أيضًا

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف.

```csharp
public void SetSource(FileInfo fileInfo)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileInfo | FileInfo | المرجع إلى ملف سيتم ضغطه. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## أمثلة

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.uue");
}
```

### انظر أيضًا

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

يضبط المحتوى الذي سيتم ترميزه داخل الأرشيف.

```csharp
public void SetSource(string path)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى الملف الذي سيتم ترميزه. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| ArgumentNullException | *path* فارغ. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول. |
| ArgumentException | المسار *path* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *path*. |
| PathTooLongException | الـ *path* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *path* يحتوي على نقطتين (:) في وسط السلسلة. |

## أمثلة

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


