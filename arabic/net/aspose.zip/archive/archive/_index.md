---
title: Archive
second_title: Aspose.ZIP لمرجع .NET API
description: يقوم بتهيئة مثيل جديد لملفArchiveaspose.zip/archiveفئة مع إعدادات اختيارية لإدخالاتها.
type: docs
weight: 10
url: /ar/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

يقوم بتهيئة مثيل جديد لملف[`Archive`](../../archive)فئة مع إعدادات اختيارية لإدخالاتها.

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | إعدادات الضغط والتشفير المستخدمة حديثًا[`ArchiveEntry`](../../archiveentry)items. إذا لم يتم تحديدها ، فسيتم استخدام ضغط Deflate الأكثر شيوعًا بدون تشفير. |

### أمثلة

يوضح المثال التالي كيفية ضغط ملف واحد بالإعدادات الافتراضية.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### أنظر أيضا

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* مساحة الاسم [Aspose.Zip](../../archive)
* المجسم [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`Archive`](../../archive) يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف.

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| sourceStream | Stream | مصدر الأرشيف. |
| loadOptions | ArchiveLoadOptions | خيارات لتحميل الأرشيف الحالي مع. |
| newEntrySettings | ArchiveEntrySettings | إعدادات الضغط والتشفير المستخدمة حديثًا[`ArchiveEntry`](../../archiveentry)items. إذا لم يتم تحديدها ، فسيتم استخدام ضغط Deflate الأكثر شيوعًا بدون تشفير. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentException | *sourceStream* لا يمكن البحث عنه. |
| InvalidDataException | يتعارض رأس التشفير لـ AES مع طريقة ضغط WinZip. |

### ملاحظات

لا يقوم المُنشئ هذا بفك ضغط أي إدخال. نرى[`Open`](../../archiveentry/open) طريقة فك الضغط.

### أمثلة

يستخرج المثال التالي أرشيفًا مشفرًا ، ثم قم بفك ضغط الإدخال الأول إلى ملف`MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### أنظر أيضا

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* مساحة الاسم [Aspose.Zip](../../archive)
* المجسم [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`Archive`](../../archive) يمكن استخراج فئة ويؤلف قائمة إدخالات من الأرشيف.

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | المسار المؤهل بالكامل أو النسبي لملف الأرشيف. |
| loadOptions | ArchiveLoadOptions | خيارات لتحميل الأرشيف الحالي مع. |
| newEntrySettings | ArchiveEntrySettings | إعدادات الضغط والتشفير المستخدمة حديثًا[`ArchiveEntry`](../../archiveentry)items. إذا لم يتم تحديدها ، فسيتم استخدام ضغط Deflate الأكثر شيوعًا بدون تشفير. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *path* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول |
| ArgumentException | ال*path* فارغ أو يحتوي على مسافات بيضاء فقط أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | الوصول إلى الملف*path* مرفوض. |
| PathTooLongException | المحدد*path*أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ، ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | ملف في*path* يحتوي على نقطتين (:) في منتصف السلسلة. |

### ملاحظات

لا يقوم المُنشئ هذا بفك ضغط أي إدخال. نرى[`Open`](../../archiveentry/open) طريقة فك الضغط.

### أمثلة

يستخرج المثال التالي أرشيفًا مشفرًا ، ثم قم بفك ضغط الإدخال الأول إلى ملف`MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### أنظر أيضا

* class [ArchiveLoadOptions](../../archiveloadoptions)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* مساحة الاسم [Aspose.Zip](../../archive)
* المجسم [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
