---
title: "AppleArchive.CreateEntry"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "AppleArchive طريقة. ينشئ مدخلاً واحدًا داخل الأرشيف"
type: docs
weight: 60
url: /ar/net/aspose.zip.apple/applearchive/createentry/
---
## CreateEntry(string, string, bool) {#createentry_2}

ينشئ مدخلًا واحدًا داخل الأرشيف.

```csharp
public AppleArchiveEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم المدخل. |
| المسار | String | المسار إلى الملف المراد ضغطه. |
| openImmediately | Boolean | صحيح، إذا تم فتح الملف فورًا، وإلا يتم فتح الملف عند حفظ الأرشيف. |

### قيمة الإرجاع

مثال كائن مدخل Apple Archive.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف. |
| ArgumentException | *name* فارغ. |
| ArgumentNullException | *path* هو `null`. |

### انظر أيضًا

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

ينشئ مدخلًا واحدًا داخل الأرشيف.

```csharp
public AppleArchiveEntry CreateEntry(string name, Stream source)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم المدخل. |
| المصدر | تيار | دفق الإدخال للمدخل. |

### قيمة الإرجاع

مثال كائن مدخل Apple Archive.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف. |
| ArgumentException | *name* فارغ. |
| ArgumentNullException | *source* هو `null`. |

### انظر أيضًا

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

ينشئ مدخلًا واحدًا داخل الأرشيف.

```csharp
public AppleArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم المدخل. |
| fileInfo | FileInfo | البيانات الوصفية للملف المراد ضغطه. |
| openImmediately | Boolean | صحيح، إذا تم فتح الملف فورًا، وإلا يتم فتح الملف عند حفظ الأرشيف. |

### قيمة الإرجاع

مثال كائن مدخل Apple Archive.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ObjectDisposedException | تم التخلص من الأرشيف. |
| ArgumentException | *name* فارغ. |
| ArgumentNullException | *fileInfo* هو `null`. |

### انظر أيضًا

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


