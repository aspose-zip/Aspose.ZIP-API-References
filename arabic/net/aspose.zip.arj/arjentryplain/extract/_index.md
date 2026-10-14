---
title: "ArjEntryPlain.Extract"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة ArjEntryPlain. تستخرج العنصر إلى نظام الملفات باستخدام المسار المقدم"
type: docs
weight: 40
url: /ar/net/aspose.zip.arj/arjentryplain/extract/
---
## Extract(string) {#extract}

يستخرج الإدخال إلى نظام الملفات باستخدام المسار المقدم.

```csharp
public FileInfo Extract(string path)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى ملف الوجهة. إذا كان الملف موجودًا بالفعل، فسيتم استبداله. |

### قيمة الإرجاع

معلومات الملف لملف مركب.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *path* هو null أو فارغ. |
| ObjectDisposedException | يتم إلقاؤه إذا تم التخلص من الأرشيف. |
| FileNotFoundException | الملف غير موجود. |
| InvalidDataException | عدم تطابق المجموع الاختباري للرؤوس أو البيانات. - أو - الأرشيف تالف. |
| PathTooLongException | المسار المحدد أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. |
| NotImplementedException | الإدخال مضغوط باستخدام الطريقة 4. |

## أمثلة

استخراج عنصرين من أرشيف rar.

```csharp
using (FileStream arjFile = File.Open("archive.arj", FileMode.Open))
{
    using (ArjArchive archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract("first.bin");
        archive.Entries[1].Extract("second.bin");
    }
}
```

### انظر أيضًا

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

يستخرج إدخال أرشيف ARJ إلى ملف.

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
| ObjectDisposedException | يتم إلقاؤه إذا تم التخلص من الأرشيف. |
| InvalidDataException | عدم تطابق المجموع الاختباري للرؤوس أو البيانات. - أو - الأرشيف تالف. |
| NotImplementedException | الإدخال مضغوط باستخدام الطريقة 4. |

## أمثلة

```csharp
using (var arjFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### انظر أيضًا

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
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
| InvalidDataException | عدم تطابق المجموع الاختباري للرؤوس أو البيانات. - أو - الأرشيف تالف. |
| NotImplementedException | الإدخال مضغوط باستخدام الطريقة 4. |
| OperationCanceledException | في .NET Framework 4.0 وما فوق: يتم إلقاء الاستثناء عندما يتم إلغاء الاستخراج عبر رمز الإلغاء المقدم. |
| ObjectDisposedException | يتم إلقاؤه إذا تم التخلص من الأرشيف. |

### انظر أيضًا

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)


