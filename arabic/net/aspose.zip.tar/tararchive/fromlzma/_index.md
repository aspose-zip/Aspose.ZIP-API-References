---
title: "TarArchive.FromLZMA"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة TarArchive. تستخرج الأرشيف LZMA المقدم وتُكوّن TarArchive من البيانات المستخرجة"
type: docs
weight: 50
url: /ar/net/aspose.zip.tar/tararchive/fromlzma/
---
## FromLZMA(Stream) {#fromlzma}

تستخرج الأرشيف LZMA المقدم وتُكوّن [`TarArchive`](../) من البيانات المستخرجة.

مهم: يتم استخراج أرشيف LZMA بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتواه داخليًا. احذر من استهلاك الذاكرة.

```csharp
public static TarArchive FromLZMA(Stream source)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | تيار | مصدر الأرشيف. |

### قيمة الإرجاع

مثال من [`TarArchive`](../)

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidDataException | الأرشيف تالف. |
| EndOfStreamException | يتم إلقاؤه عندما يتم الوصول إلى نهاية الدفق قبل قراءة عدد البايتات المتوقع. |
| ObjectDisposedException | يُرمى إذا تم التخلص من تدفق المصدر. |
| ArgumentNullException | *source* فارغ. |
| IOException | حدث خطأ في الإدخال/الإخراج. |

## ملاحظات

تيار استخراج LZMA غير قابل للتمرير بسبب طبيعة خوارزمية الضغط. يوفر أرشيف Tar إمكانية استخراج سجل عشوائي، لذا يجب أن يعمل على تيار قابل للتمرير تحت الغطاء.

### انظر أيضًا

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZMA(string) {#fromlzma_1}

تستخرج الأرشيف LZMA المقدم وتُكوّن [`TarArchive`](../) من البيانات المستخرجة.

مهم: يتم استخراج أرشيف LZMA بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتواه داخليًا. احذر من استهلاك الذاكرة.

```csharp
public static TarArchive FromLZMA(string path)
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
| EndOfStreamException | يتم إلقاؤه عندما يتم الوصول إلى نهاية الدفق قبل قراءة عدد البايتات المتوقع. |
| IOException | حدث خطأ إدخال/إخراج أثناء فتح الملف. |
| InvalidDataException | الأرشيف تالف. |

## ملاحظات

تيار استخراج LZMA غير قابل للتمرير بسبب طبيعة خوارزمية الضغط. يوفر أرشيف Tar إمكانية استخراج سجل عشوائي، لذا يجب أن يعمل على تيار قابل للتمرير تحت الغطاء.

### انظر أيضًا

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


