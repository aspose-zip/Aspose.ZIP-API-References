---
title: ZArchive.SetSource
second_title: Aspose.ZIP لمرجع .NET API
description: ZArchive طريقة. يحدد المحتوى المراد ضغطه داخل الأرشيف.
type: docs
weight: 50
url: /ar/net/aspose.zip.z/zarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

يحدد المحتوى المراد ضغطه داخل الأرشيف.

```csharp
public void SetSource(Stream source)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| source | Stream | دفق الإدخال للأرشيف. |

### أمثلة

```csharp
using (var archive = new ZArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.Z");
}
```

### أنظر أيضا

* class [ZArchive](../)
* مساحة الاسم [Aspose.Zip.Z](../../zarchive/)
* المجسم [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

يحدد المحتوى المراد ضغطه داخل الأرشيف.

```csharp
public void SetSource(FileInfo fileInfo)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo الذي سيتم فتحه كدفق إدخال. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| SecurityException | المتصل ليس لديه الإذن المطلوب لفتح*fileInfo*. |
| ArgumentException | مسار الملف فارغ أو يحتوي على مسافات بيضاء فقط. |
| FileNotFoundException | لم يتم العثور على الملف. |
| UnauthorizedAccessException | مسار الملف للقراءة فقط أو هو دليل. |
| ArgumentNullException | *fileInfo* باطل. |
| DirectoryNotFoundException | المسار المحدد غير صالح ، مثل وجوده على محرك أقراص غير معين. |
| IOException | الملف مفتوح بالفعل. |

### أمثلة

```csharp
using (var archive = new ZArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bin.Z");
}
```

### أنظر أيضا

* class [ZArchive](../)
* مساحة الاسم [Aspose.Zip.Z](../../zarchive/)
* المجسم [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

يحدد المحتوى المراد ضغطه داخل الأرشيف.

```csharp
public void SetSource(string sourcePath)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| sourcePath | String | مسار الملف الذي سيتم فتحه كمدخلات تدفق. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *sourcePath* سلسلة فارغة أو فارغة. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول إلى مورد. |
| ArgumentException | ال*sourcePath* فارغ أو يحتوي على مسافات بيضاء فقط أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | الوصول إلى الملف*sourcePath* مرفوض. |
| PathTooLongException | المحدد*sourcePath*أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ، ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | ملف في*sourcePath* يحتوي على نقطتين (:) في منتصف السلسلة. |

### أمثلة

```csharp
using (var archive = new ZArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("data.bin.Z");
}
```

### أنظر أيضا

* class [ZArchive](../)
* مساحة الاسم [Aspose.Zip.Z](../../zarchive/)
* المجسم [Aspose.Zip](../../../)


