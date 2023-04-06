---
title: AesEcryptionSettings.AesEcryptionSettings
second_title: Aspose.ZIP لمرجع .NET API
description: AesEcryptionSettings البناء. يقوم بتهيئة مثيل جديد لملفAesEcryptionSettings فئة .
type: docs
weight: 10
url: /ar/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`AesEcryptionSettings`](../) فئة .

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| password | String | كلمة مرور للتشفير أو فك التشفير. |
| method | EncryptionMethod | خيار خوارزمية يشير إلى حجم كتلة التشفير. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| NotSupportedException | *method* ليس واحدًا منAES128 وAES192 ، أوAES256. |

### أمثلة

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### أنظر أيضا

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../aesecryptionsettings/)
* المجسم [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

يقوم بتهيئة مثيل جديد لملف[`AesEcryptionSettings`](../)فئة بدون كلمة مرور.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| method | EncryptionMethod | خيار خوارزمية يشير إلى حجم كتلة التشفير. |

### أنظر أيضا

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../aesecryptionsettings/)
* المجسم [Aspose.Zip](../../../)


