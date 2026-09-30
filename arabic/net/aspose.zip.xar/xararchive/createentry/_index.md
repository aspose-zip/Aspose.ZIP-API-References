---
title: "XarArchive.CreateEntry"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة XarArchive. إنشاء إدخال واحد داخل الأرشيف"
type: docs
weight: 40
url: /ar/net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم المدخل. |
| fileInfo | FileInfo | بيانات التعريف للملف أو المجلد المراد ضغطه. |
| openImmediately | Boolean | صحيح، إذا تم فتح الملف فورًا، وإلا يتم فتح الملف عند حفظ الأرشيف. |
| compressionSettings | XarCompressionSettings | إعدادات الضغط المستخدمة للعنصر [`XarEntry`](../../xarentry/) المضاف. |

### قيمة الإرجاع

مثيل إدخال Xar.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *name* فارغ. |
| ArgumentException | *name* فارغ. |
| ArgumentNullException | *fileInfo* هو null. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## ملاحظات

إذا تم فتح الملف فوراً باستخدام المعامل *openImmediately* يصبح محجوزاً حتى يتم تحرير الأرشيف.

## أمثلة

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### انظر أيضًا

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم المدخل. |
| sourcePath | String | المسار إلى الملف الذي سيُضغط. |
| openImmediately | Boolean | صحيح، إذا تم فتح الملف فورًا، وإلا يتم فتح الملف عند حفظ الأرشيف. |
| compressionSettings | XarCompressionSettings | إعدادات الضغط المستخدمة للعنصر [`XarEntry`](../../xarentry/) المضاف. |

### قيمة الإرجاع

مثيل إدخال Xar.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *sourcePath* فارغ. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول. |
| ArgumentException | *sourcePath* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. - أو - اسم الملف، كجزء من *name*، يتجاوز 100 رمز. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *sourcePath*. |
| PathTooLongException | الـ *sourcePath* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. - أو - *name* طويل جدًا لـ xar. |
| NotSupportedException | الملف في *sourcePath* يحتوي على نقطتين (: ) في وسط السلسلة. |
| InvalidOperationException | من المستحيل تعديل أرشيف xar. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## ملاحظات

يتم تعيين اسم الإدخال فقط من خلال معامل *name*. اسم الملف المقدم في معامل *sourcePath* لا يؤثر على اسم الإدخال.

إذا تم فتح الملف فوراً باستخدام المعامل *openImmediately* يصبح محجوزاً حتى يتم تحرير الأرشيف.

## أمثلة

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### انظر أيضًا

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم المدخل. |
| المصدر | تيار | دفق الإدخال للمدخل. |
| compressionSettings | XarCompressionSettings | إعدادات الضغط المستخدمة للعنصر [`XarEntry`](../../xarentry/) المضاف. |

### قيمة الإرجاع

مثيل إدخال Xar.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *name* فارغ. |
| ArgumentNullException | *source* فارغ. |
| ArgumentException | *name* فارغ. |
| InvalidOperationException | من المستحيل تعديل أرشيف xar. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## أمثلة

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### انظر أيضًا

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


