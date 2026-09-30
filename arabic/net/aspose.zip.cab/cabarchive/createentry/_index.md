---
title: "CabArchive.CreateEntry"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة CabArchive. إنشاء إدخال واحد داخل الأرشيف"
type: docs
weight: 40
url: /ar/net/aspose.zip.cab/cabarchive/createentry/
---
## CreateEntry(string, string, CabEntrySettings) {#createentry_3}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public CabEntry CreateEntry(string name, string path, CabEntrySettings newEntrySettings = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم المدخل. |
| المسار | String | الاسم المؤهل بالكامل للملف الجديد، أو اسم الملف النسبي الذي سيتم ضغطه. |
| newEntrySettings | CabEntrySettings | إعدادات الضغط والتشفير المستخدمة للعنصر [`CabEntry`](../../cabentry/) المضاف. |

### قيمة الإرجاع

كائن إدخال Cab.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *path* فارغ. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول. |
| ArgumentException | المسار *path* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *path*. |
| PathTooLongException | الـ *path* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *path* يحتوي على نقطتين (:) في وسط السلسلة. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| InvalidOperationException | الأرشيف مُعد للاستخراج ولا يمكنه إضافة إدخالات. |

## ملاحظات

يتم تعيين اسم الإدخال فقط داخل معامل *name*. اسم الملف المقدم في معامل *path* لا يؤثر على اسم الإدخال.

## أمثلة

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.cab");
}
```

### انظر أيضًا

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, CabEntrySettings) {#createentry_2}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public CabEntry CreateEntry(string name, Stream source, CabEntrySettings newEntrySettings = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم المدخل. |
| المصدر | تيار | دفق الإدخال للمدخل. |
| newEntrySettings | CabEntrySettings | إعدادات الضغط والتشفير المستخدمة للعنصر [`CabEntry`](../../cabentry/) المضاف. |

### قيمة الإرجاع

كائن إدخال Cab.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| InvalidOperationException | الأرشيف مُعد للاستخراج ولا يمكنه إضافة إدخالات. |
| ArgumentNullException | *name* فارغ. |

## أمثلة

```csharp
using (var archive = new CabArchive())
{
    using (var dataStream = new MemoryStream(File.ReadAllBytes("data.bin")))
    {
        archive.CreateEntry("stream-entry.bin", dataStream);
        archive.Save("archive.cab");
    }
}
```

```csharp
using (var archive = new CabArchive())
{     
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("stream-entry.bin", dataStream, settings);
    archive.Save("archive.cab");     
}
```

### انظر أيضًا

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, CabEntrySettings) {#createentry_1}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public CabEntry CreateEntry(string name, FileInfo fileInfo, 
    CabEntrySettings newEntrySettings = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم المدخل. |
| fileInfo | FileInfo | البيانات الوصفية للملف المراد ضغطه. |
| newEntrySettings | CabEntrySettings | إعدادات الضغط والتشفير المستخدمة للعنصر [`CabEntry`](../../cabentry/) المضاف. |

### قيمة الإرجاع

كائن إدخال CAB.

### استثناءات

| استثناء | شرط |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* للقراءة فقط أو أنه دليل. |
| DirectoryNotFoundException | المسار المحدد غير صالح، مثل كونه على قرص غير مرتبط. |
| IOException | الملف مفتوح بالفعل. |
| FileNotFoundException | *fileInfo* يمثل ملفًا لا يمكن العثور عليه. |
| SecurityException | المستدعي لا يمتلك الإذن المطلوب للوصول إلى *fileInfo*. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| InvalidOperationException | الأرشيف مُعد للاستخراج ولا يمكنه إضافة إدخالات. |
| ArgumentNullException | *name* فارغ. |

## ملاحظات

يتم تعيين اسم الإدخال فقط داخل معامل *name*. اسم الملف المقدم في معامل *fileInfo* لا يؤثر على اسم الإدخال.

## أمثلة

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{
    var sourceFile = new FileInfo("logs\\log.txt");
    archive.CreateEntry("log.txt", sourceFile);
    archive.Save("archive.cab");
}
```

### انظر أيضًا

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, CabEntrySettings) {#createentry}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public CabEntry CreateEntry(string name, Func<Stream> streamProvider, 
    CabEntrySettings newEntrySettings = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم المدخل. |
| streamProvider | Func`1 | الطريقة التي توفر تدفق الإدخال للإدخال. |
| newEntrySettings | CabEntrySettings | إعدادات الضغط والتشفير المستخدمة للعنصر [`CabEntry`](../../cabentry/) المضاف. |

### قيمة الإرجاع

كائن إدخال CAB.

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | تم إنشاء الأرشيف لفك الضغط. - أو - عدد الملفات وصل إلى الحد الأقصى. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| ArgumentException | الـ *name* فارغ أو خالي. |

## أمثلة

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{    
    archive.CreateEntry("data.bin", provider);
    archive.Save("archive.cab");
}
```

### انظر أيضًا

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


