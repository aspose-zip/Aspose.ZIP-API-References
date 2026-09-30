---
title: "IsoArchive.CreateEntry"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "طريقة IsoArchive. تضيف ملفًا إلى صورة ISO"
type: docs
weight: 40
url: /ar/net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

يضيف ملفًا إلى صورة ISO.

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | مسار الملف في ISO. |
| filePath | String | مسار الملف. |

### قيمة الإرجاع

تم تكوين مدخل ISO.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | الـ *filePath* فارغ. |
| ArgumentException | الـ *filePath* فارغ، يحتوي فقط على مسافات بيضاء، أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | تم رفض الوصول إلى الملف *filePath*. |
| PathTooLongException | الـ *filePath* المحدد يتجاوز الحد الأقصى للطول المحدد من النظام. على سبيل المثال، في الأنظمة المستندة إلى Windows، يجب أن تكون المسارات أقل من 248 حرفًا، وأسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | الملف في *filePath* يحتوي على نقطتين (:) في وسط السلسلة. |
| IOException | حدث خطأ إدخال/إخراج أثناء فتح الملف. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| DirectoryNotFoundException | المسار المحدد غير صالح، (على سبيل المثال، هو على قرص غير مرتبط). |
| FileNotFoundException | الملف المحدد في *filePath* لم يُعثر عليه. |
| InvalidOperationException | الأرشيف ليس في وضع التحرير. |

### انظر أيضًا

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

يضيف ملفًا إلى صورة ISO.

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | مسار الملف في ISO. |
| المصدر | تيار | دفق يحتوي على بيانات الملف. |

### قيمة الإرجاع

تم تكوين مدخل ISO.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |
| ArgumentNullException | يُرمى عندما يكون *name* أو *source* فارغًا. |
| InvalidOperationException | الأرشيف ليس في وضع التحرير. |

### انظر أيضًا

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

يضيف ملفًا إلى صورة ISO.

```csharp
public IsoEntry CreateEntry(string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | مسار الدليل في ISO. |

### قيمة الإرجاع

تم تكوين مدخل ISO.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | `name` هو null أو فارغ. |
| InvalidOperationException | تم فتح الأرشيف للاستخراج. |
| ObjectDisposedException | تم التخلص من الأرشيف ولا يمكن استخدامه. |

### انظر أيضًا

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


