---
title: GzipArchive.SetSource
second_title: Aspose.ZIP لمرجع .NET API
description: GzipArchive طريقة. يحدد المحتوى المراد ضغطه داخل الأرشيف.
type: docs
weight: 70
url: /ar/net/aspose.zip.gzip/gziparchive/setsource/
---
## SetSource(Stream) {#setsource_2}

يحدد المحتوى المراد ضغطه داخل الأرشيف.

```csharp
public void SetSource(Stream source)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| source | Stream | دفق الإدخال للأرشيف. |

### أمثلة

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.gz");
}
```

### أنظر أيضا

* class [GzipArchive](../)
* مساحة الاسم [Aspose.Zip.Gzip](../../gziparchive/)
* المجسم [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

يحدد المحتوى المراد ضغطه داخل الأرشيف.

```csharp
public void SetSource(FileInfo fileInfo)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| fileInfo | FileInfo | الإشارة إلى الملف المراد ضغطه. |

### أمثلة

افتح أرشيفًا من دفق واستخرجه إلى ملف`MemoryStream`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.gz");
}
```

### أنظر أيضا

* class [GzipArchive](../)
* مساحة الاسم [Aspose.Zip.Gzip](../../gziparchive/)
* المجسم [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

يحدد المحتوى المراد ضغطه داخل الأرشيف.

```csharp
public void SetSource(string path)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | مسار الملف المراد ضغطه. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *path* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول. |
| ArgumentException | ال*path* فارغ أو يحتوي على مسافات بيضاء فقط أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | الوصول إلى الملف*path* مرفوض. |
| PathTooLongException | المحدد*path*أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ، ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | ملف في*path* يحتوي على نقطتين (:) في منتصف السلسلة. |

### أمثلة

افتح أرشيفًا من ملف حسب المسار واستخرجه إلى ملف`MemoryStream`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### أنظر أيضا

* class [GzipArchive](../)
* مساحة الاسم [Aspose.Zip.Gzip](../../gziparchive/)
* المجسم [Aspose.Zip](../../../)

---

## SetSource(TarArchive) {#setsource}

يحدد المحتوى المراد ضغطه داخل الأرشيف.

```csharp
public void SetSource(TarArchive tarArchive)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| tarArchive | TarArchive | أرشيف القطران المراد ضغطه. |

### ملاحظات

استخدم هذه الطريقة لتكوين أرشيف tar.gz مشترك.

### أمثلة

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var gzippedArchive = new GzipArchive())
    {
           gzippedArchive.SetSource(tarArchive);
           gzippedArchive.Save("archive.tar.gz");
    }
}
```

### أنظر أيضا

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* class [GzipArchive](../)
* مساحة الاسم [Aspose.Zip.Gzip](../../gziparchive/)
* المجسم [Aspose.Zip](../../../)


