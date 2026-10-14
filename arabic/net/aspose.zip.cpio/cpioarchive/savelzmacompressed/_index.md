---
title: "CpioArchive.SaveLZMACompressed"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة CpioArchive. تحفظ الأرشيف إلى الدفق باستخدام ضغط LZMA."
type: docs
weight: 110
url: /ar/net/aspose.zip.cpio/cpioarchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, CpioFormat) {#savelzmacompressed}

يحفظ الأرشيف إلى الدفق باستخدام ضغط LZMA.

```csharp
public void SaveLZMACompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الإخراج | تيار | دفق الوجهة. |
| cpioFormat | CpioFormat | يحدد تنسيق رأس cpio. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| NotSupportedException | الدفق لا يدعم الكتابة، أو أن الدفق مغلق بالفعل. |

## ملاحظات

*output* must be writable.

مهم: يتم إنشاء أرشيف cpio ثم ضغطه داخل هذه الطريقة، يتم الاحتفاظ بمحتواه داخليًا. احذر من استهلاك الذاكرة.

## أمثلة

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
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

## SaveLZMACompressed(string, CpioFormat) {#savelzmacompressed_1}

يحفظ الأرشيف إلى الملف عبر المسار باستخدام ضغط lzma.

```csharp
public void SaveLZMACompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | مسار الأرشيف الذي سيتم إنشاؤه. إذا كان اسم الملف المحدد يشير إلى ملف موجود، فسيتم استبداله. |
| cpioFormat | CpioFormat | يحدد تنسيق رأس cpio. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| ArgumentNullException | *path* هو `null`. |
| استثناء | يُرمى عندما يحدث خطأ في وقت التشغيل. |
| DirectoryNotFoundException | المسار المحدد غير صالح، (على سبيل المثال، هو على قرص غير مرتبط). |
| IOException | حدث خطأ في الإدخال/الإخراج. |
| PathTooLongException | المسار المحدد أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. |
| UnauthorizedAccessException | المستدعي لا يملك الإذن المطلوب. -أو- *path* يشير إلى ملف أو دليل للقراءة فقط. |

## ملاحظات

مهم: يتم إنشاء أرشيف cpio ثم ضغطه داخل هذه الطريقة، يتم الاحتفاظ بمحتواه داخليًا. احذر من استهلاك الذاكرة.

## أمثلة

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.cpio.lzma");
    }
}
```

### انظر أيضًا

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


