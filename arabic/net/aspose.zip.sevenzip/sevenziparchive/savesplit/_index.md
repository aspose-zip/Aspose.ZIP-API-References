---
title: SevenZipArchive.SaveSplit
second_title: Aspose.ZIP لمرجع .NET API
description: SevenZipArchive طريقة. يحفظ أرشيف متعدد المجلدات إلى دليل الوجهة المقدم.
type: docs
weight: 90
url: /ar/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

يحفظ أرشيف متعدد المجلدات إلى دليل الوجهة المقدم.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| destinationDirectory | String | المسار إلى الدليل حيث يتم إنشاء مقاطع الأرشيف. |
| options | SplitSevenZipArchiveSaveOptions | خيارات لحفظ الأرشيف ، بما في ذلك اسم الملف. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| InvalidOperationException | تم فتح هذا الأرشيف من المصدر الحالي. |
| ArgumentNullException | *destinationDirectory* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول إلى الدليل. |
| ArgumentException | *destinationDirectory* يحتوي على أحرف غير صالحة مثل "أو&gt; أو &lt;أو &#x7C;. |
| PathTooLongException | المسار المحدد يتجاوز الطول الأقصى المحدد من قبل النظام. |

### ملاحظات

هذه الطريقة تؤلف عدة (`ن`) اسم الملف ..7z.001 ، اسم الملف ..7z.002 ، ... ، اسم الملف .7z. (n).

لا يمكن جعل الأرشيف الحالي متعدد المجلدات.

### أمثلة

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### أنظر أيضا

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* مساحة الاسم [Aspose.Zip.SevenZip](../../sevenziparchive/)
* المجسم [Aspose.Zip](../../../)


