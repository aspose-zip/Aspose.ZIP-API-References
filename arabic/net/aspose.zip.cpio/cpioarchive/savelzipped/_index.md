---
title: "CpioArchive.SaveLzipped"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "CpioArchive method. يحفظ الأرشيف إلى الدفق باستخدام ضغط lzip"
type: docs
weight: 100
url: /ar/net/aspose.zip.cpio/cpioarchive/savelzipped/
---
## SaveLzipped(Stream, CpioFormat) {#savelzipped}

يحفظ الأرشيف إلى الدفق باستخدام ضغط lzip.

```csharp
public void SaveLzipped(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الإخراج | تيار | دفق الوجهة. |
| cpioFormat | CpioFormat | يحدد تنسيق رأس cpio. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *output* فارغ. |
| ArgumentException | *output* غير قابل للكتابة. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

## ملاحظات

*output* must be writable.

## أمثلة

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### انظر أيضًا

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLzipped(string, CpioFormat) {#savelzipped_1}

يحفظ الأرشيف إلى الملف عبر المسار باستخدام ضغط lzip.

```csharp
public void SaveLzipped(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| cpioFormat | CpioFormat | يحدد تنسيق رأس cpio. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| ArgumentException | *path* هو سلسلة بطول صفر، يحتوي فقط على مسافات بيضاء، أو يحتوي على حرف أو أكثر غير صالح كما هو معرف في InvalidPathChars. |
| ArgumentNullException | *path* هو `null`. |
| DirectoryNotFoundException | المسار المحدد غير صالح، (على سبيل المثال، هو على قرص غير مرتبط). |
| IOException | حدث خطأ في الإدخال/الإخراج. |
| PathTooLongException | المسار المحدد أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. |
| UnauthorizedAccessException | المستدعي لا يملك الإذن المطلوب. -أو- *path* يشير إلى ملف أو دليل للقراءة فقط. |

## أمثلة

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.cpio.lz");
    }
}
```

### انظر أيضًا

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


