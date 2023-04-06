---
title: Bzip2Archive.SetSource
second_title: Aspose.ZIP لمرجع .NET API
description: Bzip2Archive طريقة. يحدد المحتوى المراد ضغطه داخل الأرشيف.
type: docs
weight: 60
url: /ar/net/aspose.zip.bzip2/bzip2archive/setsource/
---
## SetSource(Stream) {#setsource_3}

يحدد المحتوى المراد ضغطه داخل الأرشيف.

```csharp
public void SetSource(Stream source)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| source | Stream | دفق الإدخال للأرشيف. |

### أمثلة

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00,0xFF }));
    archive.Save("archive.bz2");
}
```

### أنظر أيضا

* class [Bzip2Archive](../)
* مساحة الاسم [Aspose.Zip.Bzip2](../../bzip2archive/)
* المجسم [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_2}

يحدد المحتوى المراد ضغطه داخل الأرشيف.

```csharp
public void SetSource(FileInfo fileInfo)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| fileInfo | FileInfo | الإشارة إلى الملف المراد ضغطه. |

### أمثلة

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.bz2");
}
```

### أنظر أيضا

* class [Bzip2Archive](../)
* مساحة الاسم [Aspose.Zip.Bzip2](../../bzip2archive/)
* المجسم [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_4}

يحدد المحتوى المراد ضغطه داخل الأرشيف.

```csharp
public void SetSource(string path)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| path | String | مسار الملف المراد ضغطه. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | *path* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول. |
| ArgumentException | ال*path* فارغ أو يحتوي على مسافات بيضاء فقط أو يحتوي على أحرف غير صالحة. |
| UnauthorizedAccessException | الوصول إلى الملف*path* مرفوض. |
| PathTooLongException | المحدد*path*أو اسم الملف أو كلاهما يتجاوز الحد الأقصى للطول المحدد من قبل النظام. على سبيل المثال ، في الأنظمة الأساسية المستندة إلى Windows ، يجب أن تكون المسارات أقل من 248 حرفًا ، ويجب أن تكون أسماء الملفات أقل من 260 حرفًا. |
| NotSupportedException | ملف في*path* يحتوي على نقطتين (:) في منتصف السلسلة. |

### أمثلة

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### أنظر أيضا

* class [Bzip2Archive](../)
* مساحة الاسم [Aspose.Zip.Bzip2](../../bzip2archive/)
* المجسم [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource_1}

يحدد المحتوى المراد ضغطه داخل الأرشيف.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| tarArchive | TarArchive | أرشيف القطران المراد ضغطه. |
| format | TarFormat | يحدد تنسيق رأس القطران. |

### ملاحظات

استخدم هذه الطريقة لتكوين أرشيف tar.bz2 مشترك.

### أمثلة

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(tarArchive);
        bzippedArchive.Save("archive.tar.bz2");
    }
}
```

### أنظر أيضا

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Bzip2Archive](../)
* مساحة الاسم [Aspose.Zip.Bzip2](../../bzip2archive/)
* المجسم [Aspose.Zip](../../../)

---

## SetSource(CpioArchive, CpioFormat) {#setsource}

يحدد المحتوى المراد ضغطه داخل الأرشيف.

```csharp
public void SetSource(CpioArchive cpioArchive, CpioFormat format = CpioFormat.OldAscii)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| cpioArchive | CpioArchive | أرشيف Cpio المراد ضغطه. |
| format | CpioFormat | يحدد تنسيق رأس cpio. |

### ملاحظات

استخدم هذه الطريقة لتكوين أرشيف cpio.bz2 مشترك.

### أمثلة

```csharp
using (var cpioArchive = new CpioArchive())
{
    cpioArchive.CreateEntry("first.bin", "data1.bin");
    cpioArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(cpioArchive);
        bzippedArchive.Save("archive.cpio.bz2");
    }
}
```

### أنظر أيضا

* class [CpioArchive](../../../aspose.zip.cpio/cpioarchive/)
* enum [CpioFormat](../../../aspose.zip.cpio/cpioformat/)
* class [Bzip2Archive](../)
* مساحة الاسم [Aspose.Zip.Bzip2](../../bzip2archive/)
* المجسم [Aspose.Zip](../../../)


