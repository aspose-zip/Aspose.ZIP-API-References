---
title: Archive.SaveSplit
second_title: Aspose.ZIP لمرجع .NET API
description: Archive طريقة. يحفظ أرشيف متعدد المجلدات إلى دليل الوجهة المقدم.
type: docs
weight: 100
url: /ar/net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

يحفظ أرشيف متعدد المجلدات إلى دليل الوجهة المقدم.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| destinationDirectory | String | المسار إلى الدليل حيث يتم إنشاء مقاطع الأرشيف. |
| options | SplitArchiveSaveOptions | خيارات لحفظ الأرشيف ، بما في ذلك اسم الملف. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| InvalidOperationException | تم فتح هذا الأرشيف من المصدر الحالي. |
| NotSupportedException | هذا الأرشيف مضغوط بطريقة XZ ومشفّر. |
| ArgumentNullException | *destinationDirectory* باطل. |
| SecurityException | المتصل ليس لديه الإذن المطلوب للوصول إلى الدليل. |
| ArgumentException | *destinationDirectory* يحتوي على أحرف غير صالحة مثل "أو&gt; أو &lt;أو &#x7C;. |
| PathTooLongException | المسار المحدد يتجاوز الطول الأقصى المحدد من قبل النظام. |

### ملاحظات

هذه الطريقة تؤلف عدة (`ن`) files filename.z01، filename.z02، ...، filename.z (n-1)، filename.zip.

لا يمكن جعل الأرشيف الحالي متعدد المجلدات.

### أمثلة

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### أنظر أيضا

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* مساحة الاسم [Aspose.Zip](../../archive/)
* المجسم [Aspose.Zip](../../../)


