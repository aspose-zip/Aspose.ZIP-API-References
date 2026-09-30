---
title: "TarArchive.FromZstandard"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة TarArchive. تستخرج الأرشيف Zstandard المقدم وتُكوّن TarArchive من البيانات المستخرجة"
type: docs
weight: 80
url: /ar/net/aspose.zip.tar/tararchive/fromzstandard/
---
## FromZstandard(Stream) {#fromzstandard}

تستخرج الأرشيف Zstandard المقدم وتُكوّن [`TarArchive`](../) من البيانات المستخرجة.

مهم: يتم استخراج أرشيف Zstandard بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتواه داخليًا. احذر من استهلاك الذاكرة.

```csharp
public static TarArchive FromZstandard(Stream source)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | تيار | مصدر الأرشيف. |

### قيمة الإرجاع

مثال من [`TarArchive`](../)

### استثناءات

| استثناء | شرط |
| --- | --- |
| IOException | تيار Zstandard تالف أو غير قابل للقراءة. |
| InvalidDataException | البيانات تالفة. |
| EndOfStreamException | يتم إلقاؤه عندما يتم الوصول إلى نهاية الدفق قبل قراءة عدد البايتات المتوقع. |
| ObjectDisposedException | يُرمى إذا تم التخلص من تدفق المصدر. |

### انظر أيضًا

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromZstandard(string) {#fromzstandard_1}

تستخرج الأرشيف Zstandard المقدم وتُكوّن [`TarArchive`](../) من البيانات المستخرجة.

مهم: يتم استخراج أرشيف Zstandard بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتواه داخليًا. احذر من استهلاك الذاكرة.

```csharp
public static TarArchive FromZstandard(string path)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى ملف الأرشيف. |

### قيمة الإرجاع

مثال من [`TarArchive`](../)

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *path* فارغ. |
| ArgumentException | المسار *path* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *path*. |
| PathTooLongException | الـ *path* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *path* بتنسيق غير صالح. |
| DirectoryNotFoundException | المسار المحدد غير صالح، مثل كونه على قرص غير مرتبط. |
| FileNotFoundException | الملف غير موجود. |
| IOException | تيار Zstandard تالف أو غير قابل للقراءة. |
| InvalidDataException | البيانات تالفة. |
| EndOfStreamException | يتم إلقاؤه عندما يتم الوصول إلى نهاية الدفق قبل قراءة عدد البايتات المتوقع. |

### انظر أيضًا

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


