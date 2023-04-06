---
title: LzmaArchiveSettings.LzmaArchiveSettings
second_title: Aspose.ZIP لمرجع .NET API
description: LzmaArchiveSettings البناء. يقوم بتهيئة مثيل جديد لملفLzmaArchiveSettingsفئة بحجم القاموس الافتراضي  تساوي 16 ميغا بايت.
type: docs
weight: 10
url: /ar/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

يقوم بتهيئة مثيل جديد لملف[`LzmaArchiveSettings`](../)فئة بحجم القاموس الافتراضي ، تساوي 16 ميغا بايت.

```csharp
public LzmaArchiveSettings()
```

### أمثلة

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 } )
{
    archive.SetSource("data.bin);
    archive.Save(lzmaFile);
}
```

### أنظر أيضا

* class [LzmaArchiveSettings](../)
* مساحة الاسم [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* المجسم [Aspose.Zip](../../../)


