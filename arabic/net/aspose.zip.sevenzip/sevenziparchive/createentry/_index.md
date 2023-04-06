---
title: SevenZipArchive.CreateEntry
second_title: Aspose.ZIP لمرجع .NET API
description: SevenZipArchive طريقة. إنشاء إدخال واحد داخل الأرشيف.
type: docs
weight: 50
url: /ar/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| name | String | اسم الإدخال. |
| fileInfo | FileInfo | البيانات الوصفية للملف المراد ضغطه. |
| openImmediately | Boolean | صحيح إذا فتحت الملف على الفور ، وإلا فافتح الملف عند حفظ الأرشيف. |
| newEntrySettings | SevenZipEntrySettings | أضيفت إعدادات الضغط والتشفير المستخدمة[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) غرض. |

### قيمة الإرجاع

سبعة مثيل إدخال Zip.

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

إنشاء أرشيف بإدخالات مشفرة بكلمات مرور مختلفة لكل منها.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
        archive.CreateEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
        archive.CreateEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
        archive.Save(sevenZipFile);
    }
}
```

### أنظر أيضا

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* مساحة الاسم [Aspose.Zip.SevenZip](../../sevenziparchive/)
* المجسم [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_2}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| name | String | اسم الإدخال. |
| source | Stream | تيار الإدخال للدخول. |
| newEntrySettings | SevenZipEntrySettings | أضيفت إعدادات الضغط والتشفير المستخدمة[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) غرض. |
| fileInfo | FileSystemInfo | البيانات الوصفية للملف أو المجلد المراد ضغطه. |

### قيمة الإرجاع

مثيل دخول SevenZip.

### استثناءات

| استثناء | حالة |
| --- | --- |
| InvalidOperationException | كلاهما*source* و*fileInfo* لاغية أو*source*باطل و*fileInfo* لتقف على الدليل. |

### ملاحظات

تم تعيين اسم الإدخال فقط داخل*name* معامل. اسم الملف المقدم في*fileInfo* لا تؤثر المعلمة على اسم الإدخال.

*fileInfo* يمكن أن تشير إلىDirectoryInfo إذا كان الإدخال دليل.

### أمثلة

إنشاء أرشيف باستخدام الإدخال المشفر المضغوط LZMA2.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF}), new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new FileInfo("data1.bin")); 
        archive.Save(sevenZipFile);
    }
}
```

### أنظر أيضا

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* مساحة الاسم [Aspose.Zip.SevenZip](../../sevenziparchive/)
* المجسم [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_1}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| name | String | اسم الإدخال. |
| source | Stream | تيار الإدخال للدخول. |
| newEntrySettings | SevenZipEntrySettings | أضيفت إعدادات الضغط والتشفير المستخدمة[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) غرض. |

### قيمة الإرجاع

مثيل إدخال الرمز البريدي.

### أمثلة

قم بتكوين أرشيف 7z بضغط LZMA2 وتشفير جميع الإدخالات.

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### أنظر أيضا

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* مساحة الاسم [Aspose.Zip.SevenZip](../../sevenziparchive/)
* المجسم [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_3}

إنشاء إدخال واحد داخل الأرشيف.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| name | String | اسم الإدخال. |
| path | String | الاسم المؤهل بالكامل للملف الجديد ، أو اسم الملف النسبي المراد ضغطه. |
| openImmediately | Boolean | صحيح إذا فتحت الملف على الفور ، وإلا فافتح الملف عند حفظ الأرشيف. |
| newEntrySettings | SevenZipEntrySettings | أضيفت إعدادات الضغط والتشفير المستخدمة[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) غرض. |

### قيمة الإرجاع

مثيل إدخال الرمز البريدي.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *path* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول. |
| ArgumentException | ال*path* فارغ أو يحتوي على مسافات بيضاء فقط أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | الوصول إلى الملف*path* مرفوض. |
| PathTooLongException | المحدد*path*أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ، ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | ملف في*path* يحتوي على نقطتين (:) في منتصف السلسلة. |

### ملاحظات

تم تعيين اسم الإدخال فقط داخل*name* معامل. اسم الملف المقدم في*path* لا تؤثر المعلمة على اسم الإدخال.

إذا تم فتح الملف على الفور باستخدام*openImmediately* المعلمة يتم حظرها حتى يتم حفظ الأرشيف.

### أمثلة

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings())))
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### أنظر أيضا

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* مساحة الاسم [Aspose.Zip.SevenZip](../../sevenziparchive/)
* المجسم [Aspose.Zip](../../../)


