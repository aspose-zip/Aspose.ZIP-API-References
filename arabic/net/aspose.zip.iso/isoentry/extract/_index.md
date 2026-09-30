---
title: "IsoEntry.Extract"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة IsoEntry. تستخرج الإدخال إلى نظام الملفات باستخدام المسار المقدم"
type: docs
weight: 50
url: /ar/net/aspose.zip.iso/isoentry/extract/
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

كائن FileInfo يحتوي على البيانات المستخرجة.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *path* فارغ. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول. |
| ArgumentException | المسار *path* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *path*. |
| PathTooLongException | الـ *path* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *path* يحتوي على نقطتين (:) في وسط السلسلة. |
| FileNotFoundException | الملف غير موجود. |
| DirectoryNotFoundException | المسار المحدد غير صالح، مثل كونه على قرص غير مرتبط. |
| IOException | الملف مفتوح بالفعل. |
| InvalidOperationException | لم يتم قراءة رؤوس الأرشيف ومعلومات الخدمة. |

### انظر أيضًا

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

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
| NotSupportedException | يُطلق استثناء إذا لم يكن الإدخال يمثل ملفًا. |
| ArgumentException | الدفق المقدم لا يدعم الكتابة. |

### انظر أيضًا

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)


