---
title: "TarArchive.SaveLZ4Compressed"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة TarArchive. يحفظ الأرشيف إلى الدفق باستخدام ضغط LZ4"
type: docs
weight: 170
url: /ar/net/aspose.zip.tar/tararchive/savelz4compressed/
---
## SaveLZ4Compressed(Stream, TarFormat?) {#savelz4compressed}

يحفظ الأرشيف إلى الدفق باستخدام ضغط LZ4.

```csharp
public void SaveLZ4Compressed(Stream output, TarFormat? format = default)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الإخراج | تيار | دفق الوجهة. |
| التنسيق | Nullable`1 | يعرف تنسيق رأس tar. سيتم اعتبار القيمة Null كـ USTar عندما يكون ذلك ممكنًا. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *output* فارغ. |
| ArgumentException | *output* غير قابل للكتابة. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه |
| IOException | حدث خطأ في الإدخال/الإخراج. |

## ملاحظات

*output* must be writable.

## أمثلة

```csharp
using (FileStream result = File.OpenWrite("result.tar.lz4"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZ4Compressed(result);
        }
    }
}
```

### انظر أيضًا

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZ4Compressed(string, TarFormat?) {#savelz4compressed_1}

يحفظ الأرشيف إلى الملف بالمسار باستخدام ضغط LZ4.

```csharp
public void SaveLZ4Compressed(string path, TarFormat? format = default)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| التنسيق | Nullable`1 | يعرف تنسيق رأس tar. سيتم اعتبار القيمة Null كـ USTar عندما يكون ذلك ممكنًا. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| UnauthorizedAccessException | المستدعي لا يملك الإذن المطلوب. -أو- *path* يشير إلى ملف أو دليل للقراءة فقط. |
| ArgumentException | *path* هو سلسلة بطول صفر، يحتوي فقط على مسافات بيضاء، أو يحتوي على حرف أو أكثر غير صالح كما هو معرف في InvalidPathChars. |
| ArgumentNullException | *path* فارغ. |
| PathTooLongException | الـ *path* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| DirectoryNotFoundException | المسار المحدد *path* غير صالح، (على سبيل المثال، هو على قرص غير مرتبط). |
| NotSupportedException | *path* بتنسيق غير صالح. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه |
| IOException | حدث خطأ في الإدخال/الإخراج. |

## أمثلة

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZ4Compressed("result.tar.lz4");
    }
}
```

### انظر أيضًا

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


