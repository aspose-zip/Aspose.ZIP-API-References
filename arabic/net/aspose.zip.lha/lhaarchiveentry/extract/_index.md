---
title: "LhaArchiveEntry.Extract"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة LhaArchiveEntry. تستخرج إدخال أرشيف Lha إلى نظام ملفات حسب المسار"
type: docs
weight: 60
url: /ar/net/aspose.zip.lha/lhaarchiveentry/extract/
---
## Extract(string) {#extract}

يستخرج مدخل أرشيف Lha إلى نظام ملفات حسب المسار.

```csharp
public FileSystemInfo Extract(string path)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى الملف الذي سيخزن البيانات غير المضغوطة. |

### قيمة الإرجاع

FileSystemInfoInstance يحتوي على البيانات المستخرجة.

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | لم يتم قراءة رؤوس الأرشيف ومعلومات الخدمة. |
| ArgumentNullException | *path* فارغ. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول. |
| ArgumentException | المسار *path* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *path*. |
| PathTooLongException | الـ *path* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *path* يحتوي على نقطتين (:) في وسط السلسلة. |
| OperationCanceledException | في .NET Framework 4.0 وما فوق: يتم إلقاء الاستثناء عندما يتم إلغاء الاستخراج عبر رمز الإلغاء المقدم. |
| ObjectDisposedException | يُرمى إذا تم التخلص من تدفق المصدر. |
| InvalidDataException | يتم إلقاؤه عندما تكون البيانات غير صالحة أو تالفة. |

## أمثلة

```csharp
using (FileStream lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### انظر أيضًا

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

يستخرج الإدخال إلى الدفق المقدم.

```csharp
public void Extract(Stream destination)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الوجهة | تيار | دفق الوجهة. يجب أن يكون قابلًا للكتابة. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | *destination* لا يدعم الكتابة. |
| OperationCanceledException | في .NET Framework 4.0 وما فوق: يتم إلقاء الاستثناء عندما يتم إلغاء الاستخراج عبر رمز الإلغاء المقدم. |
| ObjectDisposedException | يُرمى إذا تم التخلص من تدفق المصدر. |
| InvalidDataException | يتم إلقاؤه عندما تكون البيانات غير صالحة أو تالفة. |

## ملاحظات

لا يفعل شيئًا لإدخال الدليل.

### انظر أيضًا

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

يستخرج مدخل أرشيف Lha إلى ملف.

```csharp
public void Extract(FileInfo fileInfo)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo لتخزين البيانات غير المضغوطة. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | لم يتم قراءة رؤوس الأرشيف ومعلومات الخدمة. |
| SecurityException | المستدعي لا يمتلك الإذن المطلوب لفتح *fileInfo*. |
| ArgumentException | مسار الملف فارغ أو يحتوي على مسافات فقط. |
| FileNotFoundException | الملف غير موجود. |
| UnauthorizedAccessException | المسار إلى الملف للقراءة فقط أو هو دليل. |
| ArgumentNullException | *fileInfo* هو null. |
| DirectoryNotFoundException | المسار المحدد غير صالح، مثل كونه على قرص غير مرتبط. |
| IOException | الملف مفتوح بالفعل. |
| OperationCanceledException | في .NET Framework 4.0 وما فوق: يتم إلقاء الاستثناء عندما يتم إلغاء الاستخراج عبر رمز الإلغاء المقدم. |
| ObjectDisposedException | يُرمى إذا تم التخلص من تدفق المصدر. |

## ملاحظات

لا يفعل شيئًا لإدخال الدليل.

## أمثلة

```csharp
using (var lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### انظر أيضًا

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)


