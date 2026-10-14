---
title: "AppleArchive.Save"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة AppleArchive. تحفظ الأرشيف إلى الدفق المقدم"
type: docs
weight: 90
url: /ar/net/aspose.zip.apple/applearchive/save/
---
## Save(Stream) {#save}

يحفظ الأرشيف إلى الدفق المقدم.

```csharp
public void Save(Stream output)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الإخراج | تيار | دفق الوجهة. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف. |
| ArgumentNullException | *output* هو `null`. |
| ArgumentException | *output* غير قابل للكتابة. |
| ArgumentOutOfRangeException | حجم كتلة LZ4 أو Zlib المُكوَّن ليس إيجابياً. |
| NotSupportedException | إعدادات الضغط مفقودة أو غير مدعومة، أو أن التركيب المباشر يستخدم دفقًا غير قابل للتمرير، أو أن حجم الإدخال/الأرشيف يتجاوز حدود أرشيف Apple الحالية. |

## ملاحظات

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### انظر أيضًا

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

يحفظ الأرشيف إلى ملف الوجهة المقدم.

```csharp
public void Save(string destinationFileName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| destinationFileName | String | مسار الأرشيف الذي سيتم إنشاؤه. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف. |
| ArgumentException | *destinationFileName* غير صالح. |
| ArgumentNullException | *destinationFileName* هو `null`. |
| ArgumentOutOfRangeException | حجم كتلة LZ4 أو Zlib المُكوَّن ليس إيجابياً. |
| NotSupportedException | إعدادات الضغط مفقودة أو غير مدعومة، أو أن التركيب المباشر يستخدم دفقًا غير قابل للتمرير، أو أن حجم الإدخال/الأرشيف يتجاوز حدود أرشيف Apple الحالية. |

### انظر أيضًا

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


