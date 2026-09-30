---
title: "TarArchive.FromLZ4"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة TarArchive. يستخرج الأرشيف LZ4 المقدم ويكوّن TarArchive من البيانات المستخرجة"
type: docs
weight: 30
url: /ar/net/aspose.zip.tar/tararchive/fromlz4/
---
## FromLZ4(string) {#fromlz4_1}

يستخرج الأرشيف LZ4 المقدم ويكوّن [`TarArchive`](../) من البيانات المستخرجة.

مهم: يتم استخراج أرشيف LZ4 بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتواه داخليًا. احذر من استهلاك الذاكرة.

```csharp
public static TarArchive FromLZ4(string path)
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
| SecurityException | المستدعي لا يمتلك الإذن المطلوب للوصول |
| ArgumentException | المسار *path* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *path*. |
| PathTooLongException | الـ *path* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *path* بتنسيق غير صالح. |
| DirectoryNotFoundException | المسار المحدد غير صالح، مثل كونه على قرص غير مرتبط. |
| FileNotFoundException | الملف غير موجود. |
| EndOfStreamException | الملف قصير جدًا. |
| InvalidDataException | الملف يحتوي على توقيع غير صحيح. |
| IOException | حدث خطأ إدخال/إخراج أثناء فتح الملف. |
| InvalidOperationException | تم إعداد الأرشيف للتركيب. |

## ملاحظات

دفق استخراج LZ4 غير قابل للتمرير بسبب طبيعة خوارزمية الضغط. يوفر أرشيف Tar إمكانية استخراج سجل عشوائي، لذا يجب أن يعمل على تدفق قابل للتمرير في الخلفية.

### انظر أيضًا

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZ4(Stream) {#fromlz4}

يستخرج الأرشيف LZ4 المقدم ويكوّن [`TarArchive`](../) من البيانات المستخرجة.

مهم: يتم استخراج أرشيف LZ4 بالكامل داخل هذه الطريقة، ويتم الاحتفاظ بمحتواه داخليًا. احذر من استهلاك الذاكرة.

```csharp
public static TarArchive FromLZ4(Stream source)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصدر | تيار | مصدر الأرشيف. |

### قيمة الإرجاع

مثال من [`TarArchive`](../)

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentException | لا يمكن القراءة من *source* |
| ArgumentNullException | *source* فارغ. |
| EndOfStreamException | *source* قصير جدًا. |
| InvalidDataException | الـ *source* يحتوي على توقيع غير صحيح. |
| ObjectDisposedException | يُرمى إذا تم التخلص من تدفق المصدر. |

## ملاحظات

دفق استخراج LZ4 غير قابل للتمرير بسبب طبيعة خوارزمية الضغط. يوفر أرشيف Tar إمكانية استخراج سجل عشوائي، لذا يجب أن يعمل على تدفق قابل للتمرير في الخلفية.

### انظر أيضًا

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


