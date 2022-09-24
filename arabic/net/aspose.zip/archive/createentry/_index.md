---
title: CreateEntry
second_title: Aspose.ZIP لمرجع .NET API
description: إنشاء إدخال واحد داخل الأرشيف.
type: docs
weight: 50
url: /ar/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_3}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| name | String | اسم الإدخال. |
| path | String | الاسم المؤهل بالكامل للملف الجديد ، أو اسم الملف النسبي المراد ضغطه. |
| openImmediately | Boolean | صحيح إذا فتحت الملف على الفور ، وإلا فافتح الملف عند حفظ الأرشيف. |
| newEntrySettings | ArchiveEntrySettings | تمت إضافة إعدادات الضغط والتشفير المستخدمة[`ArchiveEntry`](../../archiveentry) العنصر. |

### قيمة الإرجاع

مثيل إدخال الرمز البريدي.

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

تم تعيين اسم الإدخال فقط داخل*name* معامل. اسم الملف المقدم في*path* لا تؤثر المعلمة على اسم الإدخال.

إذا تم فتح الملف على الفور باستخدام*openImmediately* المعلمة يتم حظرها حتى يتم حفظ الأرشيف.

### أمثلة

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

* class [ArchiveEntry](../../archiveentry)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* مساحة الاسم [Aspose.Zip](../../archive)
* المجسم [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_1}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| name | String | اسم الإدخال. |
| source | Stream | تيار الإدخال للدخول. |
| newEntrySettings | ArchiveEntrySettings | تمت إضافة إعدادات الضغط والتشفير المستخدمة[`ArchiveEntry`](../../archiveentry) العنصر. |

### قيمة الإرجاع

مثيل إدخال الرمز البريدي.

### أمثلة

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### أنظر أيضا

* class [ArchiveEntry](../../archiveentry)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* مساحة الاسم [Aspose.Zip](../../archive)
* المجسم [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| name | String | اسم الإدخال. |
| fileInfo | FileInfo | البيانات الوصفية للملف المراد ضغطه. |
| openImmediately | Boolean | صحيح إذا فتحت الملف على الفور ، وإلا فافتح الملف عند حفظ الأرشيف. |
| newEntrySettings | ArchiveEntrySettings | تمت إضافة إعدادات الضغط والتشفير المستخدمة[`ArchiveEntry`](../../archiveentry) العنصر. |

### قيمة الإرجاع

مثيل إدخال الرمز البريدي.

### استثناءات

| استثناء | حالة |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* للقراءة فقط أو دليل. |
| DirectoryNotFoundException | المسار المحدد غير صالح ، مثل وجوده على محرك أقراص غير معين. |
| IOException | الملف مفتوح بالفعل. |

### ملاحظات

تم تعيين اسم الإدخال فقط داخل*name* معامل. اسم الملف المقدم في*fileInfo* لا تؤثر المعلمة على اسم الإدخال.

إذا تم فتح الملف على الفور باستخدام*openImmediately* المعلمة يتم حظرها حتى يتم حفظ الأرشيف.

### أمثلة

أنشئ أرشيفًا بإدخالات مشفرة بأساليب تشفير وكلمات مرور مختلفة لكل منهما.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
        archive.CreateEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass2", EncryptionMethod.AES128)));
        archive.CreateEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass3", EncryptionMethod.AES256)));
        archive.Save(zipFile);
    }
}
```

### أنظر أيضا

* class [ArchiveEntry](../../archiveentry)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* مساحة الاسم [Aspose.Zip](../../archive)
* المجسم [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_2}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| name | String | اسم الإدخال. |
| source | Stream | تيار الإدخال للدخول. |
| newEntrySettings | ArchiveEntrySettings | تمت إضافة إعدادات الضغط والتشفير المستخدمة[`ArchiveEntry`](../../archiveentry) العنصر. |
| fileInfo | FileSystemInfo | البيانات الوصفية للملف أو المجلد المراد ضغطه. |

### قيمة الإرجاع

مثيل إدخال الرمز البريدي.

### استثناءات

| استثناء | حالة |
| --- | --- |
| InvalidOperationException | كلاهما*source* و*fileInfo* لاغية أو*source* باطل و*fileInfo* لتقف على الدليل. |

### ملاحظات

تم تعيين اسم الإدخال فقط داخل*name* معامل. اسم الملف المقدم في*fileInfo* لا تؤثر المعلمة على اسم الإدخال.

*fileInfo* يمكن أن تشير إلىDirectoryInfo إذا كان الإدخال دليل.

### أمثلة

إنشاء أرشيف بإدخال مشفر.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF} ), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new FileInfo("data1.bin")); 
        archive.Save(zipFile);
    }
}
```

### أنظر أيضا

* class [ArchiveEntry](../../archiveentry)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings)
* class [Archive](../../archive)
* مساحة الاسم [Aspose.Zip](../../archive)
* المجسم [Aspose.Zip](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
