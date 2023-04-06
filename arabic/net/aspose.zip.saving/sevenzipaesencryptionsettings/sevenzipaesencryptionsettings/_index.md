---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: Aspose.ZIP لمرجع .NET API
description: SevenZipAESEncryptionSettings البناء. يقوم بتهيئة مثيل جديد لملفSevenZipAESEncryptionSettings فئة .
type: docs
weight: 10
url: /ar/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`SevenZipAESEncryptionSettings`](../) فئة .

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| password | String | كلمة مرور للتشفير أو فك التشفير. |

### أمثلة

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### أنظر أيضا

* class [SevenZipAESEncryptionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* المجسم [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

يقوم بتهيئة مثيل جديد لملف[`SevenZipAESEncryptionSettings`](../) فئة مع تشفير خارجي.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| cipher | SevenZipCipher | تنفيذ AES مخصص. |

### أمثلة

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### أنظر أيضا

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* مساحة الاسم [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* المجسم [Aspose.Zip](../../../)


