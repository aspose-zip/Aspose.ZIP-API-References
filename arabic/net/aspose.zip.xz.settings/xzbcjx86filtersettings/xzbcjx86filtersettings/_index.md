---
title: XzBcjX86FilterSettings.XzBcjX86FilterSettings
second_title: Aspose.ZIP لمرجع .NET API
description: XzBcjX86FilterSettings البناء. يقوم بتهيئة مثيل جديد لملفXzBcjX86FilterSettings . استخدمه لضغط الملفات والمكتبات القابلة للتنفيذ بداخلهXzArchive .
type: docs
weight: 10
url: /ar/net/aspose.zip.xz.settings/xzbcjx86filtersettings/xzbcjx86filtersettings/
---
## XzBcjX86FilterSettings constructor

يقوم بتهيئة مثيل جديد لملف[`XzBcjX86FilterSettings`](../) . استخدمه لضغط الملفات والمكتبات القابلة للتنفيذ بداخله[`XzArchive`](../../../aspose.zip.xz/xzarchive/) .

```csharp
public XzBcjX86FilterSettings()
```

### أمثلة

```csharp
XzLZMA2FilterSettings lzma2 = new XzLZMA2FilterSettings(5242880);
XzBcjX86FilterSettings bcj = new XzBcjX86FilterSettings();
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {bcj,lzma2}, 10485760, XzCheckType.Crc32);
using (XzArchive archive = new XzArchive(settings))
{
    archive.SetSource("data.bin");
    archive.Save("archive.xz");
}
```

### أنظر أيضا

* class [XzBcjX86FilterSettings](../)
* مساحة الاسم [Aspose.Zip.Xz.Settings](../../xzbcjx86filtersettings/)
* المجسم [Aspose.Zip](../../../)


