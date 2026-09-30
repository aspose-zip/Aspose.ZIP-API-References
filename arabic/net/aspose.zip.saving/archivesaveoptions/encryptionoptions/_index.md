---
title: "ArchiveSaveOptions.EncryptionOptions"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "خاصية ArchiveSaveOptions. يحصل أو يضبط إعدادات التشفير لحفظ أرشيف ZIP الموجود"
type: docs
weight: 60
url: /ar/net/aspose.zip.saving/archivesaveoptions/encryptionoptions/
---
## ArchiveSaveOptions.EncryptionOptions property

يحصل أو يضبط إعدادات التشفير لحفظ أرشيف ZIP الموجود.

```csharp
public EncryptionSettings EncryptionOptions { get; set; }
```

## ملاحظات

لا تستخدم هذه الخيارات لتكوين أرشيف مشفر عادي، استخدم [`EncryptionSettings`](../../archiveentrysettings/encryptionsettings/) بدلاً من ذلك.

غير متوافق مع [`DataDescriptorPolicy`](../datadescriptorpolicy/) التي لها القيمة ForAllFileEntries

## أمثلة

```csharp
using (var archive = new Archive("plain.zip"))
{                   
     archive.Save("encrypted.zip", new ArchiveSaveOptions() { EncryptionOptions = new AesEcryptionSettings("p@s$", EncryptionMethod.AES256) });
}
```

### انظر أيضًا

* class [EncryptionSettings](../../encryptionsettings/)
* class [ArchiveSaveOptions](../)
* namespace [Aspose.Zip.Saving](../../archivesaveoptions/)
* assembly [Aspose.Zip](../../../)


