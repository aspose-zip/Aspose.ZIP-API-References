---
title: "AppleArchive.AppleArchive"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "منشئ AppleArchive. يهيئ نسخة جديدة من فئة AppleArchive باستخدام الإعدادات المستخدمة للإدخالات المركبة"
type: docs
weight: 10
url: /ar/net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

يهيئ نسخة جديدة من الفئة [`AppleArchive`](../) باستخدام الإعدادات المستخدمة للإدخالات المركبة.

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | الإعدادات المستخدمة عند إنشاء أرشيف Apple جديد. |

### انظر أيضًا

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

يهيئ نسخة جديدة من الفئة [`AppleArchive`](../) ويُنشئ قائمة إدخالات يمكن استخراجها من الأرشيف.

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceStream | تيار | مصدر الأرشيف. |
| loadOptions | AppleArchiveLoadOptions | خيارات لتحميل الأرشيف الموجود. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *sourceStream* هو null. |
| ArgumentException | *sourceStream* غير قابل للتمرير. |
| InvalidDataException | *sourceStream* ليس أرشيف Apple صالح. |
| EndOfStreamException | تنتهي الدفق بشكل غير متوقع أثناء تحليل إدخالات الأرشيف. |

## ملاحظات

هذا المنشئ لا يفك ضغط أي إدخال. راجع طرق [`ExtractToDirectory`](../extracttodirectory/) و[`Open`](../../applearchiveentry/open/) لفك الضغط.

### انظر أيضًا

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

يهيئ نسخة جديدة من الفئة [`AppleArchive`](../) ويُنشئ قائمة إدخالات يمكن استخراجها من الأرشيف.

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المسار | String | المسار المؤهل بالكامل أو المسار النسبي إلى ملف الأرشيف. |
| loadOptions | AppleArchiveLoadOptions | خيارات لتحميل الأرشيف الموجود. |

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | *path* فارغ. |
| FileNotFoundException | الملف غير موجود. |
| InvalidDataException | *path* ليس أرشيف Apple صالح. |
| EndOfStreamException | تنتهي الدفق بشكل غير متوقع أثناء تحليل إدخالات الأرشيف. |

## ملاحظات

هذا المنشئ لا يفك ضغط أي إدخال. راجع طرق [`ExtractToDirectory`](../extracttodirectory/) و[`Open`](../../applearchiveentry/open/) لفك الضغط.

### انظر أيضًا

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


