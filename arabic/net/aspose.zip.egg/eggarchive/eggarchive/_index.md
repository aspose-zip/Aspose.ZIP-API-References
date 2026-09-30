---
title: "EggArchive.EggArchive"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "منشئ EggArchive. يهيئ نسخة جديدة من فئة EggArchive من دفق"
type: docs
weight: 10
url: /ar/net/aspose.zip.egg/eggarchive/eggarchive/
---
## EggArchive(Stream, EggArchiveLoadOptions) {#constructor}

يهيئ نسخة جديدة من الفئة [`EggArchive`](../) من دفق.

```csharp
public EggArchive(Stream stream, EggArchiveLoadOptions loadOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تيار | تيار | دفق أرشيف EGG. يجب أن يدعم الدفق القراءة والتمرير. |
| loadOptions | EggArchiveLoadOptions | خيارات لتحميل الأرشيف بها. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *stream* فارغ. |
| ArgumentException | *stream* غير قابل للقراءة والبحث. |

### انظر أيضًا

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)

---

## EggArchive(string, EggArchiveLoadOptions) {#constructor_1}

يُنشئ نسخة جديدة من الفئة [`EggArchive`](../) من مسار ملف.

```csharp
public EggArchive(string path, EggArchiveLoadOptions loadOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار إلى ملف أرشيف EGG. |
| loadOptions | EggArchiveLoadOptions | خيارات لتحميل الأرشيف بها. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *path* فارغ. |
| FileNotFoundException | الملف غير موجود. |
| SecurityException | المستدعي لا يملك الإذن المطلوب للوصول. |
| ArgumentException | المسار *path* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *path*. |
| PathTooLongException | الـ *path* المحدد، أو اسم الملف، أو كلاهما يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *path* يحتوي على نقطتين (:) في وسط السلسلة. |
| FileNotFoundException | الملف غير موجود. |
| DirectoryNotFoundException | المسار المحدد غير صالح، مثل كونه على قرص غير مرتبط. |
| IOException | الملف مفتوح بالفعل. |

### انظر أيضًا

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)


