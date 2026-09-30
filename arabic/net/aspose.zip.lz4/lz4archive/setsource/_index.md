---
title: "Lz4Archive.SetSource"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة Lz4Archive. يعيّن المحتوى الذي سيُضغط داخل الأرشيف"
type: docs
weight: 70
url: /ar/net/aspose.zip.lz4/lz4archive/setsource/
---
## SetSource(Stream) {#setsource_2}

يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف.

```csharp
public void SetSource(Stream source)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | تيار | دفق الإدخال للأرشيف. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | تم إعداد الأرشيف للاستخراج. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## أمثلة

```csharp
using (var archive = new Lz4Archive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz4");
}
```

### انظر أيضًا

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

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
| InvalidOperationException | تم إعداد الأرشيف للاستخراج. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## أمثلة

افتح أرشيفًا من دفق واستخرجه إلى `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz4");
}
```

### انظر أيضًا

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource}

يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| tarArchive | TarArchive | أرشيف Tar ليتم ضغطه. |
| التنسيق | TarFormat | يحدد تنسيق رأس tar. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| InvalidOperationException | هذا الأرشيف مُعد للاستخراج. |

## ملاحظات

استخدم هذه الطريقة لتكوين أرشيف tar.lz4 المشترك.

## أمثلة

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var lz4Archive = new Lz4Archive())
    {
        lz4Archive.SetSource(tarArchive);
        lz4Archive.Save("archive.tar.lz4");
    }
}
```

### انظر أيضًا

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

يضبط المحتوى الذي سيتم ضغطه داخل الأرشيف.

```csharp
public void SetSource(string path)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى الملف الذي سيُضغط. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *path* فارغ. |
| SecurityException | المستدعي لا يمتلك الإذن المطلوب للوصول |
| ArgumentException | المسار *path* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *path*. |
| PathTooLongException | الـ *path* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *path* يحتوي على نقطتين (:) في وسط السلسلة. |
| InvalidOperationException | هذا الأرشيف مُعد للاستخراج. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## أمثلة

افتح أرشيفًا من ملف عبر المسار واستخرجه إلى `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### انظر أيضًا

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


